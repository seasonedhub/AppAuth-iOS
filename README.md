#Seasoned's AppAuth-iOS Fork

Forked to fix Crossroad's OAuth Implementation so that it is compatible with HotSchedules' Oauth Server Implementation.

Token Exchanges on HS's servers must send client secrets over POST requests form data, rather than using BASIC AUTH. AppAuth-iOS refuses to allow this mode because the RFC says servers MUST implement the basic auth version and native apps SHOULD use it.

[Github Issue discussing the problem](https://github.com/openid/AppAuth-iOS/issues/276#issuecomment-410873214)


![AppAuth for iOS and macOS](https://rawgit.com/openid/AppAuth-iOS/master/appauth_lockup.svg)

[Original Repo/Documentation](https://github.com/openid/AppAuth-iOS)