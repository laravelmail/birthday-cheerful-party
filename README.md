# Birthday Cheerful Party

A professional email template for inviting guests to a birthday party, offering exclusive deals in the Entertainment and Hospitality industries.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Entertainment, Hospitality
- **Message Type:** Events
- **Tags:** party, birthday, exclusive offer

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/birthday-cheerful-party.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/birthday-cheerful-party/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.birthday-cheerful-party',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
