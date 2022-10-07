# rost SOON
![](https://github.com/Georg-code/rost_ch/raw/hauptast/logo.png)

Aren't you _müed_ from writing Rust programs in English? Do you like saying
"huere schafsäckel" a lot? Would you like to try something different, in an exotic and
funny-sounding language? Would you want to bring some Schwizerdütsch touch to your
programs?

**rost** (Schwizerdütsch/dütsch for _Rust_) is here to save your day, as it allows you to
write Rust programs in Swissgerman, using Swissgerman keywords, Swissgerman function names,
Swissgerman idioms.

This has been designed to be used as the official programming language to
develop the software for Ueli Murer

If you want to pay someone for this, pay the french guy. I only adapted his work. He does some nice shit. Worth a look.
[liberapay](https://liberapay.com/bnjbvr/).



**Examples sill in french will be translated soon**

### trait and impl (aka convention et réalisation)

```rust
rouille::rouille! {
    utilisons std::collections::Dictionnaire comme Dico;

    convention CléValeur {
        fonction écrire(&soi, clé: Chaine, valeur: Chaine);
        fonction lire(&soi, clé: Chaine) -> PeutÊtre<&Chaine>;
    }

    statique mutable DICTIONNAIRE: PeutÊtre<Dico<Chaine, Chaine>> = Rien;

    structure Concrète;

    réalisation CléValeur pour Concrète {
        fonction écrire(&soi, clé: Chaine, valeur: Chaine) {
            soit dico = dangereux {
                DICTIONNAIRE.prendre_ou_insérer_avec(Défaut::défaut)
            };
            dico.insérer(clé, valeur);
        }
        fonction lire(&soi, clé: Chaine) -> Résultat<PeutÊtre<&Chaine>, Chaine> {
            si soit Quelque(dico) = dangereux { DICTIONNAIRE.en_réf() } {
                Bien(dico.lire(&clé))
            } sinon {
                Arf("fetchez le dico".vers())
            }
        }
    }
}
```

## les contributions

First of all, _merci_ for considering participating to this joke, the
Swiss government and Rodger Federer will thank you later! Feel free to throw in a few identifiers
here and there, and open a pull-request against the `hauptast` (French for
`main`) branch.

Please don't introduce swear words, though: we will not excuse your French.

## but why would you do zat

1) why are you looking at this? Same reason
2) Reason 1
## Other languages
- French [rouille](https://github.com/bnjbvr/rouille)
- Dutch: [roest](https://github.com/jeroenhd/roest)
- German: [rost](https://github.com/michidk/rost)
- Polish: [rdza](https://github.com/phaux/rdza)
- Italian: [ruggine](https://github.com/DamianX/ruggine)
- Russian: [ржавчина](https://github.com/FluxIndustries/rzhavchina)
- Esperanto: [rustteksto](https://github.com/dscottboggs/rustteksto)
- Hindi: [zung](https://github.com/rishit-khandelwal/zung)
- Hungarian: [rozsda](https://github.com/jozsefsallai/rozsda)
- Chinese: [xiu (锈)](https://github.com/lucifer1004/xiu)
- Spanish: [rustico](https://github.com/UltiRequiem/rustico)
- Korean: [Nok (녹)](https://github.com/Alfex4936/nok)
- Finnish: [ruoste](https://github.com/vkoskiv/ruoste)
- Arabic: [sada](https://github.com/LAYGATOR/sada)
- Turkish: [pas](https://github.com/ekimb/pas)
- Vietnamese: [gỉ](https://github.com/Huy-Ngo/gir)
- Japanese: [sabi (錆)](https://github.com/yuk1ty/sabi)
- Danish: [rust?](https://github.com/LunaTheFoxgirl/rust-dk)
- Marathi: [gan̄ja](https://github.com/pranavgade20/ganja)
- Romanian: [rugină](https://github.com/aionescu/rugina)
- Czech: [rez](https://github.com/radekvit/rez)
- Ukrainian: [irzha](https://github.com/brokeyourbike/irzha)
- Bulgarian: [ryzhda](https://github.com/gavadinov/ryzhda)
- Slovak: [hrdza](https://github.com/TheMessik/hrdza)
- Catalan: [rovell](https://github.com/gborobio73/rovell)
- Corsican: [rughjina](https://github.com/aldebaranzbradaradjan/rughjina)
- Indonesian: [karat](https://github.com/annurdien/karat)
- Lithuanian: [rūdys](https://github.com/TruncatedDinosour/rudys)
- Greek: [skouriasmeno](https://github.com/devlocalhost/skouriasmeno)


## la license

[Öffentlichi Lizenz, wenn da druf drucks chaschs au nomal uf französisch lese](http://sam.zoy.org/lprab/),
