## Usage

```dart
  static Future<YourApiResponse?> yourApi(Map<String, dynamic> request) async {
    final response = await ApiService.makeRequest(
        'https://yourapiurl.com/endpoint', RequestType.get, request, headers);

    Map<String, dynamic> jsonMap = ApiService.getResponse(response);

    return YourApiResponse.fromJson(jsonMap);
  }
```
# nj_api_service
