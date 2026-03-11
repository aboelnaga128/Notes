API Endpoints Names for Chefo Delivery App
🏪 Restaurant APIs
text
GET    /api/restaurants                    → Get all restaurants (paginated + search)
GET    /api/restaurants/{id}              → Get restaurant by ID
GET    /api/restaurants/my-restaurant     → Get owner's restaurant
POST   /api/restaurants                   → Create restaurant
PUT    /api/restaurants/{id}              → Update restaurant
DELETE /api/restaurants/{id}              → Delete restaurant
🏬 Branch APIs
text
GET    /api/branches                          → Search branches (filters)
GET    /api/branches/{id}                     → Get branch by ID
GET    /api/branches/nearby                   → Get nearby branches (lat/lng)
GET    /api/branches/by-restaurant/{id}       → Get branches by restaurant
POST   /api/branches                          → Create branch
PUT    /api/branches/{id}                     → Update branch
DELETE /api/branches/{id}                     → Delete branch
PATCH  /api/branches/{id}/toggle-open         → Toggle open/closed status
🎁 Offer APIs
text
GET    /api/offers                        → Get all active offers (paginated)
GET    /api/offers/{id}                   → Get offer by ID
GET    /api/offers/by-branch/{branchId}   → Get offers by branch
POST   /api/offers                        → Create offer
PUT    /api/offers/{id}                   → Update offer
DELETE /api/offers/{id}                   → Delete offer
POST   /api/offers/{id}/apply             → Apply offer to order
🍽️ Menu APIs
text
GET    /api/menu/categories                          → Get all categories
GET    /api/menu/categories/{id}                     → Get category by ID
GET    /api/menu/categories/by-restaurant/{id}       → Get categories by restaurant
POST   /api/menu/categories                          → Create category
PUT    /api/menu/categories/{id}                     → Update category
DELETE /api/menu/categories/{id}                     → Delete category

GET    /api/menu/items                               → Get all menu items
GET    /api/menu/items/{id}                          → Get item by ID
GET    /api/menu/items/by-category/{id}              → Get items by category
POST   /api/menu/items                               → Create menu item
PUT    /api/menu/items/{id}                          → Update menu item
DELETE /api/menu/items/{id}                          → Delete menu item
PATCH  /api/menu/items/{id}/toggle-available         → Toggle item availability
🛒 Cart APIs
text
GET    /api/cart                          → Get my cart
POST   /api/cart/items                    → Add item to cart
PUT    /api/cart/items/{itemId}           → Update cart item quantity
DELETE /api/cart/items/{itemId}           → Remove item from cart
DELETE /api/cart                          → Clear cart
📦 Order APIs
text
GET    /api/orders                        → Get my orders (paginated)
GET    /api/orders/{id}                   → Get order by ID
GET    /api/orders/branch/{branchId}      → Get orders by branch (owner)
POST   /api/orders                        → Place order
PATCH  /api/orders/{id}/status            → Update order status
PATCH  /api/orders/{id}/cancel            → Cancel order
⭐ Review APIs
text
GET    /api/reviews/branch/{branchId}     → Get reviews by branch
POST   /api/reviews                       → Add review
PUT    /api/reviews/{id}                  → Update review
DELETE /api/reviews/{id}                  → Delete review
❤️ Favorites APIs
text
GET    /api/favorites                     → Get my favorites
POST   /api/favorites/{branchId}          → Add to favorites
DELETE /api/favorites/{branchId}          → Remove from favorites
👤 Auth APIs
text
POST   /api/auth/register                 → Register user
POST   /api/auth/login                    → Login
POST   /api/auth/refresh-token            → Refresh JWT token
POST   /api/auth/logout                   → Logout
POST   /api/auth/forgot-password          → Forgot password
POST   /api/auth/reset-password           → Reset password
GET    /api/auth/profile                  → Get my profile
PUT    /api/auth/profile                  → Update my profile
🖼️ Image APIs
text
POST   /api/images/branch/{branchId}      → Upload branch images
DELETE /api/images/{imageId}              → Delete branch image
PATCH  /api/images/{imageId}/order        → Update display order
