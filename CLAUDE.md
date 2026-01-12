# CLAUDE.md - mexi-landing

Landing page personal de Mauricio Cruz (@meximalist).

## Quick Reference

| Campo | Valor |
|-------|-------|
| **Dominio** | mexi.wtf |
| **Repo GitHub** | `mexiweb3/mexi-landing` |
| **Proyecto Vercel** | `mexi-landing` |
| **URL producción** | https://mexi.wtf |
| **Branch principal** | `master` |
| **Directorio local** | `/home/davidiego2/Documents/_active/mexi-landing/` |

## Estructura de Dominios mexi.wtf

### Sitios Hosteados (A Records → Vercel)

| Subdominio | Destino | Descripción |
|------------|---------|-------------|
| `mexi.wtf` | Vercel (76.76.21.21) | Landing principal - hub de links |
| `bw3.mexi.wtf` | Vercel (76.76.21.21) | BandaWeb3 podcast website |

### Redirects (GoDaddy Forwarding 301)

| Subdominio | Destino | Descripción |
|------------|---------|-------------|
| `call.mexi.wtf` | calendly.com/mexiweb3/intro-call | Agendar llamada |
| `isla.mexi.wtf` | theportal.to/... | Portal NFT |
| `partner.mexi.wtf` | forms.gle/... | Formulario de partners |
| `venganse.mexi.wtf` | docs.google.com/... | Invitación a evento |
| `yo.mexi.wtf` | bw3.mexi.wtf/es/about.html | Acerca de mi |

## Proyectos Incluidos

| Proyecto | URL | Status | Descripción |
|----------|-----|--------|-------------|
| **BandaWeb3** | bw3.mexi.wtf | Live | Podcast Web3 en español |
| **SpacesGuru** | spacesguru.com | Live | Transcripción de X Spaces |
| **SpacesToContent** | gumroad.com/l/txkuww | Live | Claude Code Skill ($49) |
| **Cazul** | cazul.vercel.app | Beta | Property management con IA |

## Redes Sociales

| Red | Handle/URL | Prioridad |
|-----|------------|-----------|
| X/Twitter | @meximalist | Principal |
| Instagram | @mexi.wtf | Activo |
| TikTok | @mexiweb3 | Activo |
| YouTube | @proofofvalue | Activo |
| Telegram | @mexiweb3 | Comunidad |
| LinkedIn | linkedin.com/in/mauriciocruzcpp | Creciendo |
| Spotify | [BandaWeb3 Podcast](https://open.spotify.com/show/0FJmpJIkWwUfspn1eNlCWB) | Podcast |
| GitHub | mexiweb3 | Código |

## Comunidad

| Comunidad | Link | Descripción |
|-----------|------|-------------|
| **Ethereum México** | ethmexico.org | Organización ETH en México |
| **mxweb3 WhatsApp** | chat.whatsapp.com/... | Comunidad Web3 México |
| **Participa en BandaWeb3** | Google Forms | Aplicar como invitado |

## Stack Técnico

- HTML estático + Tailwind CSS (CDN)
- Fonts: Exo 2 (headers), Inter (body)
- Deploy: Vercel (automático via GitHub)
- DNS: GoDaddy (A records + forwarding)

## Archivos

```
mexi-landing/
├── index.html          # Landing page
├── assets/
│   ├── avatar.png      # Foto de perfil
│   ├── favicon.ico     # Favicon "M" emerald
│   └── favicon.svg     # Fuente del favicon
├── vercel.json         # Config Vercel
└── CLAUDE.md           # Este archivo
```

## Comandos

```bash
# Deploy (automático con push)
git push origin master

# Preview local
python3 -m http.server 8000

# Verificar DNS
dig mexi.wtf +short
dig bw3.mexi.wtf +short
```

## DNS en GoDaddy

Para agregar nuevo subdominio hosteado en Vercel:
1. GoDaddy → DNS → Add Record
2. Tipo: A, Host: `subdominio`, Value: `76.76.21.21`
3. Vercel: `vercel domains add subdominio.mexi.wtf`

Para agregar redirect simple:
1. GoDaddy → Forwarding → Add
2. Subdominio → URL destino, Tipo: Permanente (301)

## Tareas Pendientes

- [ ] **Live Vibecodeando** - Mañana 12pm (Restream)

## Colores

| Color | Hex | Uso |
|-------|-----|-----|
| Background | #0a0a0a | Fondo principal |
| Emerald | #10b981 | Accent principal |
| Indigo | #6366f1 | Accent secundario |
| Text | #f5f5f5 | Texto principal |
| Gray | #9ca3af | Texto secundario |
