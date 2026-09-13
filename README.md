# JNX Fest Landing Page

Temporary static landing page for `jnxfest.com`, designed around the current JNX Fest handout artwork.

The page is ready for GitHub Pages. After pushing this repository to GitHub, enable Pages from the repository settings and publish from the main branch root.

## Publish Checklist

1. Create a GitHub repository, for example `jnxfest`.
2. Push this local repository to GitHub:

   ```powershell
   git remote add origin https://github.com/YOUR-USER-OR-ORG/jnxfest.git
   git push -u origin main
   ```

3. In GitHub, open **Settings > Pages** for the repository.
4. Set the source to deploy from the `main` branch root.
5. Confirm the custom domain is `jnxfest.com`.

## Cloudflare DNS

For the apex domain `jnxfest.com`, create these `A` records for `@`:

```text
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Optionally add GitHub Pages `AAAA` records for IPv6:

```text
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153
```

For `www.jnxfest.com`, create a `CNAME` record pointing to `YOUR-USER-OR-ORG.github.io`.
