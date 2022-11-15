# minimidi data

This is the dataset of TRS MIDI devices used for [minimidi.world](https://minimidi.world).

`devices.ttl` is a file in [Terse RDF Triple Language (Turtle)](https://www.w3.org/TR/turtle) syntax.

## Template

```
_:label device:make "Make" .
_:label device:model "Model" .
_:label device:inputs 1 .
_:label device:outputs 1 .
_:label device:thrus 1 .
_:label device:swappable true .
_:label device:typeA true .
_:label device:typeB true .
_:label device:notes "Brief notes about the device" .
_:label device:details "Longer detailed description" .
_:label device:uri "https://example.com" .
_:label device:eurorack true .
```

## Terms

`label` - lowercase, dash-delimited, url-friendly ASCII name for the device, usually `make-model` (see https://www.w3.org/TR/turtle/#grammar-production-PN_CHARS_BASE)

`device:make` - make of the device

`device:model` - model of the device

`device:inputs` - how many TRS MIDI inputs? (do not include DIN MIDI inputs)

`device:outputs` - how many TRS MIDI outputs? (do not include DIN MIDI outputs)

`device:thrus` - how many TRS MIDI thrus? (do not include DIN MIDI thrus)

`device:typeA` – does the device support Type A?

`device:typeB` – does the device support Type B?

`device:typeTS` - does the device support Type TS (mono)?

`device:swappable` – can the device be configured for EITHER Type A OR Type B?

`device:notes` – brief notes describing the device

`device:details` – longer details, especially regarding how the device works

`device:uri` – main official internet web page uri of the device

`device:eurorack` – (default: false) for devices available in both eurorack and non-eurorack, is this entry for a eurorack version of the device?
