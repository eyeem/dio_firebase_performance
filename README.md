# dio_firebase_performance

Dio's Interceptor implementation that sends http request metric data to Firebase.

__STATUS: works for us in production.__

## Usage

```dart
final dio = Dio();
final performanceInterceptor = DioFirebasePerformanceInterceptor();
dio.interceptors.add(performanceInterceptor);
```

__SUGGESTION:__ If you use dio client as a singleton you can use this interceptor as singleton as well.
