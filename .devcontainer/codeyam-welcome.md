# CodeYam Editor

You are inside your codespace. The CodeYam Editor runs here, on port 14199, and opens in its own browser tab.

## Opening the editor

The first time, the codespace installs the editor before starting it, which takes a few minutes. When it is ready, the editor opens in a new tab on its own.

If no tab opened, or you closed it:

1. Open the **Ports** panel, next to Terminal at the bottom of this window.
2. Find port **14199**, labelled **CodeYam Editor**.
3. Click the globe icon on that row ("Open in Browser").

Port 14199 is listed straight away, but until the editor is running it shows an error page (HTTP 502). While the codespace is still installing, watch its progress: press Ctrl+Shift+P (Cmd+Shift+P on a Mac) and run **Codespaces: View Creation Log**. If the install has finished and you still get the error, see below.

## Signing in

The first time you start the AI that builds with you, the editor asks you to sign in to it. Follow the steps on that screen.

## If the editor does not come up

Its output is in a log file. In the terminal, run:

```bash
cat .codeyam/logs/codespaces-editor.log
```

To start it yourself, run this and leave it running, then reload the editor tab (or open port 14199 from the Ports panel):

```bash
codeyam-editor start --hosted --no-open --port 14199
```

## Who can reach the editor

Only you. The port is private, so GitHub asks anyone else to sign in first and then refuses them. If you make the port public in the Ports panel, the editor starts asking for its own token.
