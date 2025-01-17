# React Js (Client Side)
### vercel.json
```json
{
    "rewrites":  [
        {
            "source": "/(.*)", 
            "destination": "/"
        }
    ]
}
```
# Express Js (Server Side)
### vercel.json
```json
{
    "version": 2,
    "builds": [
        {
            "src": "./index.js",
            "use": "@vercel/node"
        }
    ],
    "routes": [
        {
            "src": "/(.*)",
            "dest": "/",
            "methods": ["GET", "POST", "PUT", "PATCH", "DELETE", "OPTIONS"]
        }
    ]
}
```
