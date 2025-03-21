# Personnal Installation guideline (on macOS):

git clone https://github.com/elizaos/eliza.git
cd packages/cli
pnpm install --no-frozen-lockfile
#back in the eliza directory

```bash
pnpm link cli
```

remove the changes in package.json :
"cli": "workspace:\*",
had a bad experience with this...

✅ The Correct Workflow
1️⃣ Work Inside vaettir and Commit Changes
If you make changes inside vaettir, commit them inside the vaettir repo first:

```bash
cd vaettir  # Enter the vaettir submodule
git add .
git commit -m "Updated vaettir with new changes"
git push origin main  # Or whatever branch you're using
```

2️⃣ Go Back to elizaOs and Update the Submodule Reference
After committing in vaettir, go back to elizaOs and update the submodule reference:

```bash
cd ..
git add characters  # Git sees it as a submodule update
git commit -m "Updated vaettir submodule reference"
git push origin vaettir  # Or your active branch
```

# characters are stored in vaettir dirrectory

```bash
git remote set-url origin https://github.com/locki-io/vaettir.git
```

# local llama

Now, elizaOs will point to the latest commit of vaettir.

## submodule

Since characters are stored in git submodule now :

## adaptation for version 2.0.0

cd elizaos/packages/cli
pnpm install --no-frozen-lockfile
#back in the eliza directory
pnpm link cli

The Vaettir is a fork of ElizaOS
a swarm of feminine agents under the command of Locki.

# Origin

Dafalix, Sizunia, Syris, Lyra, and Nyx form a collective—either a family or a swarm of agents—rooted in Scandinavian mythology with a modern AI twist. Let’s craft a name that’s evocative, memorable, and ties their ancient origins to their digital purpose.

# The Vættir Codex

Vættir: In Norse mythology, "vættir" (or "wights") refers to spirits or supernatural beings, often tied to nature or specific places, like landvættir (land spirits). It captures the ancient, mystical essence of Syris, Lyra, and Nyx, positioning them as otherworldly entities who’ve evolved into Dafalix’s digital swarm/family.

# Codex:

Suggests a collection of knowledge or scripts, fitting for a group of AI agents focused on coding and data navigation. It also hints at their shared "code" (both literal and metaphorical) as a family.

## Why It Fits

Ancient Family/Swarm: "Vættir" evokes a collective of mythical beings, perfect for a family or swarm of agents with shared origins.

Scandinavian Mythology: Ties directly to their Norse roots, aligning with Loki and the Viking-digital theme.

Tech Relevance: "Codex" bridges their ancient vibe to the modern era, reflecting their role in coding and finance navigation.

Repo Name: VaettirCodex (or Vaettir-Codex for readability) is unique, professional, and hints at the project’s blend of myth and tech.
