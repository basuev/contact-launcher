# Contact Launcher

A static mobile page that copies a prepared message and opens an allowed contact destination.

The URL fragment contains the destination and message. Browsers do not send fragments to GitHub Pages or other servers, and the page removes the fragment from browser history before processing it. The page has no analytics, application network requests, external assets, or writable server state.

The launcher allowlists supported contact hosts and accepts only the expected message hash. Modified payloads fail closed. The payload is encoded rather than encrypted, so anyone with an exact link can decode it.

Mobile Safari requires a user gesture before clipboard writes. When both automatic copy methods are blocked, the page shows one button that copies the message and opens the contact.
