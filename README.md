# Minimal representation of xenial-vs-trusty chrome behavior in Docker

## Trusty

- [Failed build](https://travis-ci.org/soulshake/google-chrome-xenial-issue-repro#L455)

```
$ google-chrome-stable
The command "google-chrome-stable" exited with 1.
```

## Xenial

- [Failed build](https://staging.travis-ci.org/soulshake/google-chrome-xenial-issue-repro#L364)

```
$ google-chrome-stable
[2522:2522:1201/201244.055528:FATAL:setuid_sandbox_host.cc(157)] The SUID sandbox helper binary was found, but is not configured correctly. Rather than run without sandboxing I'm aborting now. You need to make sure that /opt/google/chrome/chrome-sandbox is owned by root and has mode 4755.
/home/travis/.travis/job_stages: line 57:  2522 Aborted                 (core dumped) google-chrome-stable
The command "google-chrome-stable" exited with 134.
```

## See also

- [soulshake/google-chrome-xenial-issue-repro](https://hub.docker.com/r/soulshake/google-chrome-xenial-issue-repro) minimal Docker image
