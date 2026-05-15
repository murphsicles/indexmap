# @collections/indexmap — Ordered Hash Map for Zeta

Auto-converted from [indexmap](https://crates.io/crates/indexmap) v2.14.0 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- **IndexMap** — hash map with predictable iteration order (insertion order)
- **IndexSet** — hash set with predictable iteration order
- **O(1) lookups** — same performance as HashMap/HashSet
- **Indexing** — access by index (`map[0]`, `map[5]`) for random access
- **Splice/shift** — `shift_remove`, `swap_remove`, `pop`, `retain`, `drain`
- **Sorted** — `sort_keys`, `sort_by`, `sorted_by` for temporary sorted views
- **Serde** — serialize/deserialize preserving order

## Usage
```zeta
use @collections/indexmap::IndexMap;

let mut map = IndexMap::new();
map.insert("c", 3);
map.insert("a", 1);
map.insert("b", 2);
for (key, val) in &map {
    println!("{}: {}", key, val); // c: 3, a: 1, b: 2 (insertion order)
}
```

## Stats: ~7,728 lines, 0 unsupported items

## License: MIT