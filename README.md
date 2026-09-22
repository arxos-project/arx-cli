<p align="center">
  <img src="assets/arx-icon-mark.svg" width="120" alt="Arx OS logo">
</p>

# Arx CLI

Wrapper de linha de comando do **Arx OS** — versão atual: **0.2.0**

## O que é

Um wrapper fino sobre o `apt`, com foco em conveniência e integração com o ecossistema Arx OS.

## Uso

```bash
arx install <pacote>
arx update
arx upgrade
arx search <termo>
```

Autocomplete disponível via `_apt` (Bash).

## Instalação

```bash
wget http://arxos.is-a.dev/arx-archive-keyring.deb
sudo dpkg -i arx-archive-keyring.deb

echo "deb http://arxos.is-a.dev/repo stable main" | sudo tee /etc/apt/sources.list.d/arxos.list

sudo apt update
sudo apt install arx-cli
```

## Curiosidade

```bash
arx moo
```

## Roadmap

- [ ] Checagem de origem do pacote antes de decidir exigir senha de domínio (parte da futura "loja de aplicativos", Fase 3 do Arx OS)

Um rascunho não-produtivo de regra Polkit está documentado em `polkit/10-arx-repo-installs.rules` — incompleto de propósito, aguardando a Fase 3.

## Licença

[GNU GPLv3](LICENSE)

## Contato

arxos.project@gmail.com
