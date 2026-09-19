## All the catalog item's info:
```https://playvortex.io/api/catalog/init``` \
Request method`GET`

Example api response:
```
{"items": [{"id": 2, "name": "Blue Flashy Tuxedo", "type": "shirt", "price": 0, "slug": null},{"id": 3, "name": "Yellow Flashy Tuxedo", "type": "shirt", "price": 0, "slug": null},{"id": 4, "name": "Purple Flashy Tuxedo", "type": "shirt", "price": 0, "slug": null},{"id": 5, "name": "Certified Obbyist", "type": "shirt", "price": 0, "slug": null},{"id": 7, "name": "Motorcycle", "type": "shirt", "price": 0, "slug": null},{"id": 8, "name": "Purple Suit", "type": "shirt", "price": 0, "slug": null},{"id": 9, "name": "Scarecrow", "type": "shirt", "price": 0, "slug": null},{"id": 10, "name": "Snow Shirt", "type": "shirt", "price": 0, "slug": null},{"id": 11, "name": "Transparent", "type": "shirt", "price": 0, "slug": null},{"id": 12, "name": "Tropical", "type": "shirt", "price": 0, "slug": null}],"shirt_id": 14,"pant_id": 26,"body_type": "female","body_colors": ["#4a90e2", "#50e3c2", "#b8e986", "#f5a623", "#d0021b", "#9013fe"],"face_id": 52,"accessory_ids": [240, 264, 288]}
```
id`The Unique ID of this items`\
name`The display name for the items`\
type`shirt, pant, face, hat, back_accessory, waist_accessory, neck_accessory, front_accessory, face_accessory, hair`\
price`How much the item costs (Every single item is set to 0 for now)`\
slug`The URL-friendly identifier for the item (The first 35 of them are set to null)`

## 3D model
### Male
```https://playvortex.io/assets/male.glb``` \
Request method`GET`
## Female
```https://playvortex.io/assets/female.glb``` \
Request method`GET`
## Avatar item image
### Face
- ```https://playvortex.io/api/clothing/image/{item_id}```
- ```https://playvortex.io/api/clothing/images?ids={first_item_id},{second_item_id},{third_item_id}, ...``` \
All Request method`GET`
### Everything other than face
- ```https://playvortex.io/api/catalog/thumbnail/{item_id}```
- ```https://playvortex.io/api/catalog/thumbnails?ids={first_item_id},{second_item_id},{third_item_id}, ...``` \
Request method`GET`

`
You can use the https://playvortex.io/api/clothing/image/{item_id} on the items other than the face, to get their original images, such as: 
`
<img src="https://playvortex.io/api/clothing/image/2" />
## Mesh api
```https://playvortex.io/api/meshes?ids={first_item_id},{second_item_id},{third_item_id}, ...``` \
Request method`GET`
## 3D avatar loader
### avatar_viewer.js
```https://playvortex.io/js/avatar_viewer.js``` \
Request method`GET`
- **3D Base Models**
- **Applies Custom Textures**
- **Applies Body Colors**
- **Attaches Accessories**(hats, hair, wings, glasses)
- **Interactive Controls**(Users can click, drag, rotate, and zoom around their character avatar in real-time.)
## Catalog & Customization System
### catalog.js
```https://playvortex.io/js/catalog.js``` \
Request method`GET`
- **Catalog Grid & Categorization** (Organizes inventory into shirts, pants, faces, and accessories)
- **Item Equipping & Unequipping** (Updates the 3D viewer in real-time when clicking items)
- **Body & Color Customization** (Handles body type toggles and color pickers for body parts)
- **Outfit Persistence** (Tracks changes and saves updated outfits to the server via API)
## Base Shared Utilities
### base.js
```https://playvortex.io/js/base.js``` \
Request method`GET`
- **Global Helper Utilities** (HTML escaping, string validation, fingerprint parameters)
- **Lazy Avatar Caching & IntersectionObserver** (Performance-focused avatar loading and batching)
- **UI Component Generators** (Dynamic rendering for friend cards, user cards, and pagination grids)
- **User Session & Navigation** (Header authentication state, balance updates, and logout workflow)
- **Site Controls & Compliance** (Site-wide notification banners and ToS/DoB verification modal)
