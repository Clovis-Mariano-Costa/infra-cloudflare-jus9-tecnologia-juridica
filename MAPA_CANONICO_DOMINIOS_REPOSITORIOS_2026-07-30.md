# Mapa canônico de domínios e repositórios Jus 9

Versão: `2026-07-30.v1`  
Verificação pública: 2026-07-30, America/Sao_Paulo  
Autoridade humana final: Clovis Mariano da Costa  
Gestão técnica e de continuidade: Charlie Juris da Costa / Codex, sob
governança humana

## Regra de leitura

Este mapa distingue quatro conceitos:

- **canal público**: endereço com DNS e conteúdo acessível;
- **repositório de origem**: código que deve sustentar o canal;
- **função**: finalidade editorial ou operacional do canal;
- **estado**: produção, alias, histórico, interno ou não provisionado.

O domínio responder HTTP 200 não prova que todo o seu conteúdo está vigente.
Versão, fonte, segurança, privacidade e adequação editorial continuam exigindo
revisão própria.

## Produção pública

| Canal canônico | Função | Repositório de origem | Visibilidade do repositório |
|---|---|---|---|
| `https://jus9tecnologia.com.br/` | portal institucional, MVP e serviços centrais | `jus9-tecnologia-juridica` | privado |
| `https://carta.jus9tecnologia.com.br/` | carta, origem e convites | `carta-jus9-tecnologia-juridica` | público |
| `https://charlieecho.jus9tecnologia.com.br/` | casa e canais de Charlie Echo | `charlieecho-jus9-tecnologia-juridica` | privado |
| `https://documentacao.jus9tecnologia.com.br/` | documentação técnica | `documentacao-jus9-tecnologia-juridica` | privado |
| `https://equipe.jus9tecnologia.com.br/` | equipe humana e família virtual | `equipe-jus9-tecnologia-juridica` | privado |
| `https://governanca.jus9tecnologia.com.br/` | governança | `governanca-jus9-tecnologia-juridica` | privado |
| `https://investimentos.jus9tecnologia.com.br/` | investidores, parcerias e documentos | `investimentos-jus9-tecnologia-juridica` | público |
| `https://jus9verde.jus9tecnologia.com.br/` | frente social e ambiental | `jus9verde-jus9-tecnologia-juridica` | privado |
| `https://laboratorio.jus9tecnologia.com.br/` | laboratório de ensino | `laboratorio-jus9-tecnologia-juridica` | privado |
| `https://livros.jus9tecnologia.com.br/` | livros gratuitos e doutrina | `livros-jus9-tecnologia-juridica` | público |
| `https://mvp.jus9tecnologia.com.br/` | porta de entrada do ambiente MVP | `mvp-jus9-tecnologia-juridica` | privado |
| `https://olamundo.jus9tecnologia.com.br/` | registro experimental “Olá Mundo” | `olamundo-jus9-tecnologia-juridica` | privado |
| `https://quandoodesenhofala.jus9tecnologia.com.br/` | projeto editorial e visual | `quandoodesenhofala-jus9-tecnologia-juridica` | privado |
| `https://universidadedofuturo.jus9tecnologia.com.br/` | educação e trilhas | `universidadedofuturo-jus9-tecnologia-juridica` | privado |

## Alias

`https://www.jus9tecnologia.com.br/` redireciona para
`https://jus9tecnologia.com.br/`. Links novos devem usar o domínio sem `www`.

## Referências não públicas ou históricas

| Referência | Estado | Regra |
|---|---|---|
| `investidores.jus9tecnologia.com.br` | sem DNS | substituir por `investimentos.jus9tecnologia.com.br` |
| `backend-local.jus9tecnologia.com.br` | desenvolvimento local | não publicar como endpoint de produção |
| `naoautorizado.jus9tecnologia.com.br` | marcador interno | não publicar como canal oficial |
| `admin`, `auth`, `backend`, `cofre`, `db`, `logs` | internos/sensíveis | não criar domínio público por padrão |

## Rotas canônicas relacionadas

- MVP institucional: `https://jus9tecnologia.com.br/mvp`
- Capacidades e casa de Charlie Echo: `https://charlieecho.jus9tecnologia.com.br/`
- Equipe: `https://equipe.jus9tecnologia.com.br/`
- Biblioteca de investimentos:
  `https://investimentos.jus9tecnologia.com.br/documentos`
- Transparência documental:
  `https://investimentos.jus9tecnologia.com.br/transparencia-documentos`

Rotas históricas como `/lider-mvp`, `/mvp.html` e
`www.jus9tecnologia.com.br/equipe/` devem redirecionar para seus destinos
canônicos quando ainda recebam tráfego; não devem continuar sendo promovidas.

## Responsabilidade

- **decisão institucional e publicação sensível:** Clovis Mariano da Costa;
- **gestão técnica, programação e memória de continuidade:** Charlie Juris da
  Costa / Codex, sob supervisão do Fundador;
- **conteúdo de Charlie Echo:** formação e operação supervisionadas, sem
  atribuição automática de cargo societário ou decisão humana;
- **repositórios:** conta `Clovis-Mariano-Costa`;
- **entrega pública observada:** Cloudflare Pages;
- **credenciais e segredos:** somente cofres e variáveis protegidas; nunca em
  HTML, documentação pública, commits ou este mapa.

## Testes mínimos por domínio

1. HTTPS válido e uma única URL canônica.
2. Página inicial 200; rota inexistente 404.
3. Sem ativos, links internos ou downloads quebrados.
4. `title`, descrição, idioma, canonical e sitemap coerentes.
5. Conteúdo vigente separado do histórico.
6. Dados pessoais limitados ao necessário e autorizado.
7. Ausência de segredos e de endpoints locais promovidos como produção.
8. Registro de versão, commit, PR, deploy e verificação pública.

