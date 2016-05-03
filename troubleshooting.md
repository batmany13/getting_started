### Troubleshotting Guide

### mix test fails with error
`** (CompileError) test/controllers/login_controller_test.exs:2: module Brighterlink.ConnCase is not loaded and could not be found
    (elixir) expanding macro: Kernel.use/1
    test/controllers/login_controller_test.exs:2: Brighterlink.LoginControllerTest (module)
    (elixir) lib/code.ex:363: Code.require_file/2
    (elixir) lib/kernel/parallel_require.ex:47: anonymous fn/2 in Kernel.ParallelRequire.spawn_requires/5`

I ran into this when I had set my MIX_ENV=dev on my local, and tried to run mix test.  The problem is "conn_case" is a test environment, and if you run mix test with the wrong ENV, it doesn't know to build it for test, and thus it was missing the file in the _build/test directory.