
NFramework generators for the `nfw` CLI toolchain. Generators render with (http://crates.io/crates/tera) and are consumed by the [nfw CLI](../nfw). The catalog is declared in [`nfw.catalog.yaml`](nfw.catalog.yaml).

---

## Generators

| Identifier        | Display Name                      | Description                                                    |
| ----------------- | --------------------------------- | -------------------------------------------------------------- |
| `blank-workspace` | Blank Workspace                   | Minimal starter workspace                                      |
| `dotnet-service`  | .NET Service (Clean Architecture) | .NET service with Domain/Application/Infrastructure/Api layers |

---

## Usage

Generators are resolved by the `nfw` CLI. See the [nfw CLI README](../nfw) for details.

```bash
# List discovered generators
nfw generators list

# Create a workspace from a generator
nfw new my-workspace --generator blank-workspace

# Scaffold a .NET service
nfw add service Orders --generator dotnet-service
```

---

## Build & Test

```bash
make build
make test
```

## Format & Lint

```bash
make format
make lint
```

---

## 📄 License

This project is licensed under the **Apache License 2.0** - see the [LICENSE](LICENSE) file for details.
