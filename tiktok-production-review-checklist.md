# TikTok Production Review Checklist

Use this checklist before resubmitting the TikTok Developer production review.

## Public URLs

- Website URL points to the deployed `docs/index.html` site.
- Privacy Policy URL points to `docs/privacy.html`.
- Terms of Service URL points to `docs/terms.html`.
- All submitted URLs are publicly reachable without login.
- The website is not a placeholder, construction page, empty repository page, or
  localhost URL.

## Website Content

- The homepage explains what Video Bot does.
- The homepage explains how TikTok Login Kit is used.
- The homepage explains how the Content Posting API is used.
- The homepage lists the TikTok scopes requested by the app.
- The homepage explains that generated videos are reviewed before upload.
- The homepage includes visible links to Terms of Service and Privacy Policy.

## TikTok App Configuration

- Redirect URI exactly matches the value used by the app.
- Requested scopes match the implementation:
  - `user.info.basic`
  - `video.upload`
  - `video.publish`
- App review notes explain both upload modes:
  - `video.upload` sends a video to TikTok inbox/draft flow.
  - `video.publish` uses Direct Post for approved generated videos.

## Suggested Review Note

Video Bot is a desktop creator tool used by the authorized account owner to
generate, review, and publish short vertical videos. The app uses TikTok Login
Kit for OAuth authorization and TikTok Content Posting API for video upload and
Direct Post. The requested scopes are `user.info.basic`, `video.upload`, and
`video.publish`. Generated videos are stored locally and can be reviewed before
publishing. The public website describes the product, TikTok integration,
security practices, privacy policy, and terms of service.
