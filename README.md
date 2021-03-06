# Enarx Demos
Programs for demonstrating the Enarx subcomponents and eventually their synergy.

## AMD SEV
A demonstration of running encrypted code in an SEV VM.

## Wasmtime Basic
Compiling either a C or Rust program to WASM and running it natively using a Rust-powered JIT.

## [Wasmtime - Rust native in WASM](wasmtime-native-embed)
Running native Rust code in a WASM virtual machine without pre-compiling it.

## Intel SGX
A demonstration of remote attestation for an SGX enclave. The attesting enclave prepares a Report for the platform's
Quoting Enclave, which verifies the Report and signs it with its Attestation Key, producing a Quote. The Quote is
sent off-platform to the tenant, who can verify the Quote with a certificate chain from Intel. An attestation daemon
(located on the enclave's same platform) communicates between the tenant and enclave.
