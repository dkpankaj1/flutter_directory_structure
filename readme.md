lib/
├── main.dart
├── app/                          # App-level configuration
│   ├── app.dart                  # Main app widget
│   ├── routes/                   # Route definitions
│   │   ├── app_routes.dart
│   │   └── route_names.dart
│   └── themes/                   # App themes
│       ├── app_theme.dart
│       ├── light_theme.dart
│       └── dark_theme.dart
├── core/                         # Core functionality
│   ├── constants/                # App constants
│   │   ├── api_constants.dart
│   │   ├── app_constants.dart
│   │   └── storage_constants.dart
│   ├── errors/                   # Error handling
│   │   ├── exceptions.dart
│   │   ├── failures.dart
│   │   └── error_handler.dart
│   ├── network/                  # Network layer
│   │   ├── api_client.dart
│   │   ├── dio_client.dart
│   │   ├── interceptors/
│   │   │   ├── auth_interceptor.dart
│   │   │   ├── logging_interceptor.dart
│   │   │   └── error_interceptor.dart
│   │   └── network_info.dart
│   ├── services/                 # Core services
│   │   ├── storage_service.dart
│   │   ├── notification_service.dart
│   │   └── dependency_injection.dart
│   └── utils/                    # Core utilities
│       ├── validators.dart
│       ├── formatters.dart
│       ├── extensions.dart
│       └── helpers.dart
├── shared/                       # Shared components
│   ├── widgets/                  # Reusable widgets
│   │   ├── common/
│   │   │   ├── custom_button.dart
│   │   │   ├── custom_text_field.dart
│   │   │   ├── loading_widget.dart
│   │   │   └── error_widget.dart
│   │   └── inputs/
│   │       ├── form_field_wrapper.dart
│   │       └── custom_dropdown.dart
│   └── models/                   # Shared data models
│       ├── base_model.dart
│       └── response_model.dart
├── features/                     # Feature-based organization
│   ├── auth/
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   │   ├── auth_local_datasource.dart
│   │   │   │   └── auth_remote_datasource.dart
│   │   │   ├── models/
│   │   │   │   ├── auth_model.dart
│   │   │   │   ├── user_model.dart
│   │   │   │   └── login_response_model.dart
│   │   │   └── repositories/
│   │   │       └── auth_repository_impl.dart
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   │   ├── user_entity.dart
│   │   │   │   └── auth_entity.dart
│   │   │   ├── repositories/
│   │   │   │   └── auth_repository.dart
│   │   │   └── usecases/
│   │   │       ├── login_usecase.dart
│   │   │       ├── logout_usecase.dart
│   │   │       ├── register_usecase.dart
│   │   │       └── get_current_user_usecase.dart
│   │   └── presentation/
│   │       ├── providers/
│   │       │   └── auth_provider.dart
│   │       ├── screens/
│   │       │   ├── login_screen.dart
│   │       │   ├── register_screen.dart
│   │       │   └── profile_screen.dart
│   │       └── widgets/
│   │           ├── auth_form_field.dart
│   │           └── social_login_buttons.dart
│   └── todos/
│       ├── data/
│       │   ├── datasources/
│       │   │   ├── todo_local_datasource.dart
│       │   │   └── todo_remote_datasource.dart
│       │   ├── models/
│       │   │   ├── todo_model.dart
│       │   │   └── todo_response_model.dart
│       │   └── repositories/
│       │       └── todo_repository_impl.dart
│       ├── domain/
│       │   ├── entities/
│       │   │   └── todo_entity.dart
│       │   ├── repositories/
│       │   │   └── todo_repository.dart
│       │   └── usecases/
│       │       ├── get_todos_usecase.dart
│       │       ├── create_todo_usecase.dart
│       │       ├── update_todo_usecase.dart
│       │       └── delete_todo_usecase.dart
│       └── presentation/
│           ├── providers/
│           │   └── todo_provider.dart
│           ├── screens/
│           │   ├── todo_list_screen.dart
│           │   ├── todo_detail_screen.dart
│           │   └── add_todo_screen.dart
│           └── widgets/
│               ├── todo_item_widget.dart
│               ├── todo_form_widget.dart
│               └── todo_filter_widget.dart
└── l10n/                         # Internationalization (optional)
    ├── app_localizations.dart
    └── arb/
        ├── app_en.arb
        └── app_es.arb
