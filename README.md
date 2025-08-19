# ytimage
Allows for **image comments in YouTube** by parsing `image[...]` tags and embedding Imgur images.  
This only works for users with the Tampermonkey script/extension installed.

---

## Config
Configuration is built into the script as a JSON-like object.

- **reveal-blacklist**  
  Shows blacklisted images as blurred images, which can be revealed by clicking.  
  Default: `false`  

- **reveal-nonwhitelist**  
  Shows images not in the whitelist as blurred images.  
  Default: `true`  

- **auto-unhide-nonwhitelist**  
  Requires `reveal-nonwhitelist=true`. Automatically unblurs images that aren’t whitelisted.  
  Default: `false`  

- **regex**  
  Regex used to detect and extract image tags.  
  Default:  
  ```json
  {"regex": "image\\[(.*?)\\]"}
