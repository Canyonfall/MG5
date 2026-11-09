# MG5
## Devlog
Put your Devlog here.

A NavMesh is useful when a character needs to choose a path through a level and navigate around obstacles without the player controlling every step. For instance, in an imagined real-time strategy game where a player clicks a destination for a villager, and the villager should find a walkable route around buildings. A NavMeshAgent will fit that behavior because it allow follow a path on the baked walkable surface. Besides, physics-based movement is more useful when forces, momentum, gravity, and collisions are calculated to influence how the character moves. For instance, an imagined 3D marble-rolling platformer would benefit from Rigidbody-based movement, since slopes, rolling, bumps, and falling should affect the ball's motion. 


The corrected loop starts at index 0, and checks that i < _birds.Length, and increases i by one after each iteration. As a result, it visits every entry in the _birds array, including the first bird and the last bird, without accessing an index beyond the array's length. For each bird, Vector3.Distance(bird.transform.position, _player.position) calculates the straight-line distance between bird and Pudu. The if statement compares this distance with _interactDistance. If the distance is less than or equal to the interaction distance the script will call bird.RunAway(_player.position), telling that bird to run from the player's position. In this way, every assigned bird within the interaction distance runs away. And Birds farther away do not receive that call. 

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [Mountain fantasy environment models](https://www.fab.com/listings/60487a72-3f20-4bb2-aa78-247ed1582656)
