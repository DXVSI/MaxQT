# MaxQT

**MaxQT** - специализированный клиент для Max.ru, построенный на Qt WebEngine. Предоставляет нативный опыт рабочего стола с интеграцией в системный трей и поддержкой уведомлений.

<div align="center">
  <img src="maxqt.png" alt="MaxQt Icon" width="300" height="300">
</div>

[![Linux](https://img.shields.io/badge/OS-Linux-blue.svg)](https://www.linux.org/) [![Qt6](https://img.shields.io/badge/Qt-6-green.svg)](https://www.qt.io/) [![C++](https://img.shields.io/badge/Language-C%2B%2B-orange.svg)](https://isocpp.org/)

## ✨ Особенности

- 🖥️ **Нативное приложение** - полная интеграция с рабочим столом Linux
- 🔔 **Системные уведомления** - получайте уведомления через D-Bus
- 📱 **Системный трей** - минимизация в трей для быстрого доступа
- ⚡ **Высокая производительность** - оптимизировано для работы с Max.ru
- 🔐 **Безопасность** - изолированная среда Flatpak

## 📦 Установка

### Из Flatpak (рекомендуется)

1. Скачайте последний релиз `MaxQt.flatpak` из [Releases](https://github.com/DXVSI/MaxQT/releases)
2. Установите:
   ```bash
   flatpak install MaxQt.flatpak
   ```

### Запуск приложения

```bash
# Из меню приложений или командной строки
flatpak run org.maxqt.MaxQt
```

## 🐛 Устранение неполадок

### Проблемы с аудио/PulseAudio

Если видите ошибки PulseAudio, добавьте права доступа:

```bash
flatpak override --user --socket=pulseaudio org.maxqt.MaxQt
```

### Проблемы с системным треем

Убедитесь, что ваше DE поддерживает системный трей:

- **GNOME**: установите расширение `TopIcons Plus`
- **KDE**: трей должен работать по умолчанию
- **XFCE**: включите панель уведомлений

## 📄 Лицензия

Этот проект использует следующие лицензии:

- **Исходный код**: GPLv3+
- **Qt WebEngine**: LGPL-3.0
- **Документация**: MIT

## 👨‍💻 Разработчик

**DXVSI** - [GitHub](https://github.com/DXVSI)

## 📞 Поддержка

- **Issues**: [GitHub Issues](https://github.com/DXVSI/MaxQT/issues)

## 📈 Версии

Текущая версия: **1.0.0**

---

**Сделано с ❤️ для сообщества Max.ru**
