# shell-iq

**shell-iq** is an AI-powered tool that watches the `stdio` and `stderr` from a shell process and provides concise summaries of errors and successes. It’s particularly useful for accelerating development by analyzing server or test output, allowing you to quickly identify and understand failures without manually digging through long logs.

## Features

- AI-powered log summarization
- AI-powered suggestions for test failures
- Monitors `stdout` and `stderr` from your shell processes
- Provides clear, succinct reports of errors and successes
- Saves time when reviewing long and complex logs from servers or tests

## Installation

You can install shell-iq via npm:

```bash
npm install -g shell-iq
```

Alternatively, you can run it via `npx`:

```bash
npx shell-iq -- your-command
```

## Usage

Before running `shell-iq`, ensure that you have your OpenAI API key available as an environment variable:

```bash
export OPENAI_API_KEY=your-api-key
```

To run your command and have `shell-iq` monitor it, use the following command:

```bash
./shell-iq -- your-command
```

Replace `your-command` with the actual command you want to run and monitor.

### Example:

```bash
export OPENAI_API_KEY=xyz
./shell-iq -- npm run test
```

In this example, `shell-iq` will monitor the output of your test command and provide a concise summary of errors and successes.

## License

MIT# shell-iq
