This is a fork of [erlang/OTP](https://github.com/erlang/otp/) with patches to make compilation on modern C standards possible. 
If you have run into compilation issues using `asdf install erlang 24...` or other older versions, this might be for you. 

I have created some branches called `OTP-...-patched` for the versions I specifically need. 
The only difference to the base version is two or so changed lines of C code. 

To use this patched verion in ASDF you will have to do the following:

```
# original command:
asdf install erlang 24.3.3      # 24.3.3 is an example version

# use this instead:
export OTP_GITHUB_URL="https://github.com/nirit100/otp"
asdf instal erlang ref:OTP-24.3.3-patched
```

... or in your `.tool-versions` file:

```
erlang ref:OTP-24.3.3-patched
```

You do not have to use my fork, you can just patch the files yourself. Maybe this was helpful anyways. Who knows.

Ok bye

---

To see the erlang repository code, switch to one of the branches.
