# Django-chunked-queryset-iterator
The function slices a queryset into smaller querysets containing chunk_size objects and then yield them. It is used to avoid memory error when processing huge queryset, and also database error due to that the database pulls whole table at once. Concurrent database modification wouldn't make some entries repeated or skipped in this process.
