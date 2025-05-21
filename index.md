# Onderzoek naar DNS

![DNS](https://www.lifewire.com/thmb/-EmyFPpQ6Dpo9kBb9XV-sdgR9I4=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/GettyImages-585297068-52005387a57248a19e3ee29bc1af44b4.jpg)

## Inhoudsopgave
- [Wat is DNS?](#wat-is-dns)
- [Hoe werkt DNS?](#hoe-werkt-dns)
- [De rol van DNS op het internet](#de-rol-van-dns-op-het-internet)
- [Veiligheid en risico's](#veiligheid-en-risicos)
- [Tabel: Veelvoorkomende DNS-aanvallen](#tabel-veelvoorkomende-dns-aanvallen)
- [Bronnen](#bronnen)

---

## Wat is DNS?

DNS staat voor **Domain Name System**.

Het vertaalt domeinnamen zoals `www.nike.com` naar IP-adressen zoals `23.10.171.131`.

## Hoe werkt DNS?

Wanneer je `www.nike.com` bezoekt:

1. Je browser vraagt het IP-adres aan je besturingssysteem.
2. Het OS vraagt het aan een **DNS-resolver** (bijv. van Ziggo).
3. De resolver vraagt bij een **rootserver** (zoals Verisign).
4. De rootserver verwijst naar een **TLD-server** (zoals de `.com` server).
5. De TLD-server verwijst naar Nike’s **authoritative nameserver** (bijv. `ns1.p24.dynect.net`).
6. Die stuurt het IP-adres terug.
7. Je browser maakt verbinding met dat IP-adres.

Je kunt dit zelf testen via [digwebinterface.com](https://www.digwebinterface.com).

## De rol van DNS op het internet

DNS zorgt ervoor dat het internet gebruiksvriendelijk is. Niemand hoeft IP-adressen te onthouden.

## Veiligheid en risico's

Standaard is DNS niet veilig. Zonder beveiliging kunnen hackers verkeer omleiden (**DNS spoofing**). Oplossingen zijn:
- DNSSEC
- DNS over HTTPS (DoH)

### Gevaren bij inbraak

Als hackers DNS-verkeer manipuleren, kunnen ze:
- Je doorsturen naar nepwebsites
- Je wachtwoorden stelen
- Je gegevens onderscheppen

## Tabel: Veelvoorkomende DNS-aanvallen

| Aanvalstype        | Uitleg                            | Gevolg                                 |
|--------------------|-----------------------------------|-----------------------------------------|
| DNS Spoofing       | Nepantwoord sturen                | Verkeerde website geladen               |
| Cache Poisoning    | DNS-cache vervalsen               | Verkeerde routing van gebruikers        |
| DNS Amplification  | DNS-verzoek misbruiken            | Grootschalige DDoS-aanvallen            |

## Externe link

Meer info bij [ICANN](https://www.icann.org/)

## Bronnen

- Cloudflare. (z.d.). *What is DNS?* https://www.cloudflare.com/learning/dns/what-is-dns/  
- ICANN. https://www.icann.org/  
- Wikipedia. *DNS*. https://nl.wikipedia.org/wiki/Domain_Name_System
