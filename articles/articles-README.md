# Articles

This folder contains article data for Lucas's portfolio website.

## 📝 How to Submit an Article

### Step 1: Prepare Your Content

Write your article content in sections with these types:
- `paragraph` - Regular text
- `heading2` - Main section headings
- `heading3` - Subsection headings
- `blockquote` - Pull quotes or important callouts

### Step 2: Add to articles.json

Open `articles.json` and add your article to the `articles` array:

```json
{
  "slug": "your-article-slug",
  "title": "Your Article Title",
  "subtitle": "A compelling subtitle that describes what readers will learn",
  "category": "Design Systems",
  "date": "October 22, 2025",
  "readTime": "8 min read",
  "author": "Lucas Sublime",
  "featuredImage": "https://your-image-url.com/image.jpg",
  "tags": ["Tag 1", "Tag 2", "Tag 3"],
  "content": [
    {
      "type": "paragraph",
      "text": "Your opening paragraph introducing the topic."
    },
    {
      "type": "heading2",
      "text": "Main Section Title"
    },
    {
      "type": "paragraph",
      "text": "Content under this section."
    },
    {
      "type": "heading3",
      "text": "Subsection Title"
    },
    {
      "type": "paragraph",
      "text": "More detailed content."
    },
    {
      "type": "blockquote",
      "text": "An important quote or key takeaway to highlight."
    }
  ],
  "relatedArticles": [
    "slug-of-related-article-1",
    "slug-of-related-article-2"
  ]
}
```

### Step 3: Field Explanations

**Required Fields:**
- `slug` - URL-friendly identifier (e.g., "why-design-matters")
- `title` - Article title
- `subtitle` - Brief description (1-2 sentences)
- `category` - Article category
- `date` - Publication date (Month Day, Year)
- `readTime` - Estimated reading time
- `author` - Author name
- `featuredImage` - Hero image URL (1000x600px recommended)
- `tags` - Array of topic tags
- `content` - Array of content blocks (see Step 2)

**Optional Fields:**
- `relatedArticles` - Array of slugs for related articles

### Step 4: Content Block Types

Each content block needs a `type` and `text`:

```json
{ "type": "paragraph", "text": "Regular paragraph text" }
{ "type": "heading2", "text": "Main Section Heading" }
{ "type": "heading3", "text": "Subsection Heading" }
{ "type": "blockquote", "text": "Important quote or callout" }
```

### Step 5: Slug Guidelines

- Use lowercase letters
- Replace spaces with hyphens
- No special characters
- Keep it short and descriptive
- Example: "Building Design Systems" → `building-design-systems`

### Step 6: Image Requirements

- **Featured Image:** 1000x600px (or 5:3 aspect ratio)
- Format: JPG or PNG
- File size: Under 500KB for performance
- Host on reliable CDN or image hosting service

### Step 7: Testing

After adding your article:
1. Commit and push to GitHub
2. Visit: `yoursite.dev/article?slug=your-article-slug`
3. Check all content displays correctly
4. Test dark mode toggle
5. Verify related articles load

### 💡 Tips

- Keep paragraphs focused (3-5 sentences)
- Use heading2 for main sections, heading3 for subsections
- Add blockquotes for key takeaways
- Aim for 5-10 content blocks per article
- Include 2-3 related articles for better navigation
- Write compelling subtitles - they appear in previews

### 🔗 Article URLs

Articles are accessed via:
```
yoursite.dev/article?slug=your-article-slug
```

Each article gets its own URL based on the slug you define.
