# 🎛️ Kill Switch Config

Control remoto para tu sitio WordPress.

## URL del JSON

```
https://Dalvae.github.io/dalvae-killswitch/killswitch.json
```

## Configuración en WordPress

Agrega a tu `wp-config.php`:

```php
define('KILLSWITCH_REMOTE_URL', 'https://Dalvae.github.io/dalvae-killswitch/killswitch.json');
```

## Estructura del JSON

```json
{
  "enabled": false,        // true = activar kill switch
  "mode": "maintenance",   // maintenance | degraded | hidden
  "message": "Mensaje",    // Mensaje para usuarios
  "show_theme": true       // false = mostrar página de mantenimiento
}
```

## Activar mantenimiento

1. Edita `killswitch.json`
2. Cambia `"enabled": false` a `"enabled": true`
3. Cambia `"show_theme": true` a `"show_theme": false`
4. Commitea y pushea
5. Espera max 5 minutos (o refresca desde admin bar)

