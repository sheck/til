---
title: "::Kernel.binding.pry"
date: 2020-03-05 23:45:00 Z
---

If you’re using `binding.pry` in a delegator and (frustratingly) find yourself in the `def method_missing` context, you can use `::Kernel.binding.pry` instead and it will place your context in the ⚡️ right spot ⚡️