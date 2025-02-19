# Elixir Enum.each and Process.exit

This example showcases a potential issue when abruptly terminating a process within an `Enum.each` loop.  The loop continues normally, but the process exits before the loop has completed.  This can lead to unexpected behavior and difficult-to-debug errors. The solution provides a more robust method of handling this behavior.