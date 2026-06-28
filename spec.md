# JPCandles — Landing Page Design Specification

## 1. Expanded Prompt

### Project Context
- **Brand:** JPCandles — premium handmade candles
- **Story:** Artisan-crafted candles made with love, natural ingredients, and attention to detail. Each candle is a unique piece of functional art.
- **Mood:** Warm, organic, intimate, luxurious yet approachable
- **Intent:** Showcase handmade candle collection, communicate quality and craftsmanship, drive engagement/sales

### Hero Section
- **Pattern:** Video-Led Hero
- **Visual:** Warm, soft cinematic video of candlelight flickering — slow-motion close-up of a hand lighting a candle, warm amber glow filling the frame
- **Overlay:** Minimal text — brand name + tagline floating in negative space
- **Resolution:** 1080p minimum, cinematic quality

### Typography
- **Headline:** Bold, elegant serif (e.g., Playfair Display or similar) — large, dramatic scale
- **Body:** Clean sans-serif (e.g., Inter or similar) — readable, modern
- **Strategy:** Contrast between serif headings (luxury feel) and sans-serif body (modern clarity). Hero text at 4rem+ on desktop, scaling down responsively.

### Layout
- **Grid:** Full-width sections with generous whitespace
- **Rhythm:** 80px vertical padding between sections on desktop
- **Structure:** Hero → About → Collection → Craftsmanship → Testimonials → CTA → Footer

### Motion
- **Scroll:** Subtle fade-in animations on scroll (IntersectionObserver)
- **Hover:** Smooth scale on product cards, warm glow on buttons
- **Transitions:** 0.4s ease for all interactive elements
- **Parallax:** Gentle parallax on hero video

## 2. Tech Strategy

### Stack
- HTML5 (semantic)
- CSS3 (custom properties, grid, flexbox, animations)
- Vanilla JS (IntersectionObserver for scroll animations, minimal)
- Google Fonts (Playfair Display + Inter)

### Asset Protocol
- Hero video: Cinematic candlelight close-up, warm amber tones, 1080p, looped
- Images: Product shots with warm, natural lighting
- Format: MP4 for video, WebP for images

## 3. Design System

### Color Palette (Earth tones — NO blue/purple)
| Token | Hex | Usage |
|---|---|---|
| `--bg-primary` | `#1a1410` | Dark background (hero, footer) |
| `--bg-secondary` | `#f5efe8` | Light sections (about, collection) |
| `--bg-tertiary` | `#ede4d8` | Card backgrounds, alternating sections |
| `--text-primary` | `#f5efe8` | Light text on dark |
| `--text-secondary` | `#3d2e1f` | Dark text on light |
| `--text-muted` | `#8a7560` | Subtitles, captions |
| `--accent` | `#c8956c` | Warm amber — buttons, links, highlights |
| `--accent-hover` | `#d4a87e` | Hover states |
| `--glow` | `#e8b97a` | Candlelight glow effect |
| `--divider` | `#d4c4b0` | Subtle borders, separators |

### Typography
| Token | Value | Usage |
|---|---|---|
| `--font-heading` | `'Playfair Display', serif` | All headings |
| `--font-body` | `'Inter', sans-serif` | Body text, navigation |
| `--hero-size` | `clamp(3rem, 8vw, 7rem)` | Hero headline |
| `--heading-1` | `clamp(2.5rem, 5vw, 4.5rem)` | Section headings |
| `--heading-2` | `clamp(1.5rem, 3vw, 2.5rem)` | Card headings |
| `--body` | `1.125rem` | Body text |
| `--small` | `0.875rem` | Captions, labels |

### Layout Tokens
| Token | Value | Usage |
|---|---|---|
| `--container-max` | `1200px` | Max content width |
| `--section-pad` | `clamp(60px, 10vh, 120px)` | Vertical section padding |
| `--gap` | `24px` | Grid gap |
| `--radius` | `12px` | Card border radius |

## 4. Sections

### Hero
- Full viewport video background (warm candlelight close-up)
- Dark overlay (rgba 26, 20, 16, 0.4)
- Centered text: "JPCandles" (hero size) + "Handcrafted with warmth" (subtitle)
- CTA button: "Explore Collection"
- Scroll indicator (animated arrow)

### About
- Light background (`--bg-secondary`)
- Two-column layout: text + image
- Story of craftsmanship, natural ingredients, handmade process

### Collection
- Light background
- Grid of 6 product cards (3x2 desktop, 2x3 tablet, 1x6 mobile)
- Each card: image, name, description, price
- Hover: subtle scale + warm glow shadow

### Craftsmanship
- Dark background (`--bg-primary`)
- Process steps: 4 steps shown horizontally (desktop) / vertically (mobile)
- Icons or minimal illustrations
- Warm accent lines connecting steps

### Testimonials
- Light background (`--bg-tertiary`)
- 3 testimonial cards in a row
- Quote, author, star rating
- Elegant quotation mark decoration

### CTA
- Dark background with warm gradient
- Large heading: "Experience the warmth"
- Subtitle: "Handcrafted candles for your home"
- CTA button: "Shop Now"

### Footer
- Dark background
- Brand name, social links, copyright
- Minimal, clean
