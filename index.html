import 'package:flutter/material.dart';

void main() => runApp(SovaGoodbyeApp());

class SovaGoodbyeApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      theme: ThemeData(
        primaryColor: const Color(0xFF58CC02),
        scaffoldBackgroundColor: Colors.white,
        fontFamily: 'Roboto',
      ),
      home: MainNavigationScreen(),
    );
  }
}

class Task {
  final String russianText;
  final List<String> correctOrder;
  final List<String> availableWords;

  Task({
    required this.russianText,
    required this.correctOrder,
    required this.availableWords,
  });
}

class Flashcard {
  final String english;
  final String russian;
  Flashcard({required this.english, required this.russian});
}

class UserProfile {
  static String userName = 'Честный Студент';
  static int totalXP = 0;
  static int currentLevel = 1;
  static int completedLessons = 0;
  static int streakFreezes = 0;
  static bool doubleXpActive = false;

  static List<Map<String, dynamic>> leaderboard = [
    {'name': 'Анна', 'xp': 140},
    {'name': 'Иван', 'xp': 90},
    {'name': 'Alex_Pro', 'xp': 60},
    {'name': 'Сова_Убийца', 'xp': 30},
    {'name': 'Елена', 'xp': 10},
  ];

  static void addXP(int amount) {
    int finalAmount = doubleXpActive ? amount * 2 : amount;
    totalXP += finalAmount;
    currentLevel = (totalXP / 150).floor() + 1;
    _updateLeaderboard();
  }

  static void _updateLeaderboard() {
    bool found = false;
    for (var user in leaderboard) {
      if (user['name'] == userName) {
        user['xp'] = totalXP;
        found = true;
      }
    }
    if (!found) {
      leaderboard.add({'name': userName, 'xp': totalXP});
    }
    leaderboard.sort((a, b) => (b['xp'] as int).compareTo(a['xp'] as int));
  }
}

class MainNavigationScreen extends StatefulWidget {
  @override
  _MainNavigationScreenState createState() => _MainNavigationScreenState();
}

class _MainNavigationScreenState extends State<MainNavigationScreen> {
  int _currentIndex = 0;

  @override
  Widget build(BuildContext context) {
    final List<Widget> _screens = [
      HomeScreen(),
      ProfileScreen(), // Убрал сложный колбэк обновления, теперь стейт обновляется локально
      ShopScreen(),
    ];

    return Scaffold(
      body: _screens[_currentIndex],
      bottomNavigationBar: Container(
        decoration: BoxDecoration(
          border: Border(
            top: BorderSide(color: Colors.grey.shade200, width: 2),
          ),
        ),
        child: BottomNavigationBar(
          currentIndex: _currentIndex,
          selectedItemColor: const Color(0xFF58CC02),
          unselectedItemColor: Colors.grey.shade400,
          selectedFontSize: 14,
          unselectedFontSize: 14,
          type: BottomNavigationBarType.fixed,
          backgroundColor: Colors.white,
          elevation: 0,
          onTap: (index) {
            setState(() {
              _currentIndex = index;
            });
          },
          items: const [
            BottomNavigationBarItem(
              icon: Icon(Icons.school, size: 28),
              label: 'Обучение',
            ),
            BottomNavigationBarItem(
              icon: Icon(Icons.person, size: 28),
              label: 'Профиль',
            ),
            BottomNavigationBarItem(
              icon: Icon(Icons.shopping_bag, size: 28),
              label: 'Магазин',
            ),
          ],
        ),
      ),
    );
  }
}

class HomeScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text(
          'Сова, Гудбай',
          style: TextStyle(
            color: Color(0xFF3C3C3C),
            fontWeight: FontWeight.w900,
            fontSize: 24,
          ),
        ),
        backgroundColor: Colors.white,
        elevation: 0,
        actions: [
          Container(
            margin: const EdgeInsets.only(right: 16, top: 12, bottom: 12),
            padding: const EdgeInsets.symmetric(horizontal: 12, vertical: 4),
            decoration: BoxDecoration(
              color: Colors.orange.shade50,
              borderRadius: BorderRadius.circular(12),
            ),
            child: Row(
              children: [
                const Text('⚡', style: TextStyle(fontSize: 18)),
                const SizedBox(width: 4),
                Text(
                  '${UserProfile.totalXP} XP',
                  style: const TextStyle(
                    fontWeight: FontWeight.bold,
                    color: Colors.orange,
                    fontSize: 14,
                  ),
                ),
              ],
            ),
          ),
        ],
      ),
      body: Center(
        child: SingleChildScrollView(
          padding: const EdgeInsets.all(24),
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
            children: [
              ElevatedButton.icon(
                style: ElevatedButton.styleFrom(
                  backgroundColor: Colors.amber.shade400,
                  elevation: 0,
                  shape: RoundedRectangleBorder(
                    borderRadius: BorderRadius.circular(12),
                  ),
                  padding: const EdgeInsets.symmetric(
                    horizontal: 20,
                    vertical: 12,
                  ),
                ),
                icon: const Icon(Icons.leaderboard, color: Colors.white),
                label: const Text(
                  'РЕЙТИНГ ЛИГИ',
                  style: TextStyle(
                    color: Colors.white,
                    fontWeight: FontWeight.bold,
                    fontSize: 16,
                  ),
                ),
                onPressed: () {
                  Navigator.push(
                    context,
                    MaterialPageRoute(
                      builder: (context) => LeaderboardScreen(),
                    ),
                  );
                },
              ),
              const SizedBox(height: 40),
              GestureDetector(
                onTap: () {
                  Navigator.push(
                    context,
                    MaterialPageRoute(builder: (context) => LessonScreen()),
                  ).then((_) {
                    (context as Element).markNeedsBuild();
                  });
                },
                child: Container(
                  width: 130,
                  height: 130,
                  decoration: BoxDecoration(
                    color: const Color(0xFF58CC02),
                    shape: BoxShape.circle,
                    border: Border.all(
                      color: const Color(0xFF46A302),
                      width: 6,
                    ),
                    boxShadow: [
                      BoxShadow(
                        color: const Color(0xFF58CC02).withOpacity(0.3),
                        blurRadius: 20,
                        offset: const Offset(0, 8),
                      ),
                    ],
                  ),
                  child: const Column(
                    mainAxisAlignment: MainAxisAlignment.center,
                    children: [
                      Text('👋🦉', style: TextStyle(fontSize: 42)),
                      SizedBox(height: 4),
                      Text(
                        'ТЕСТ',
                        style: TextStyle(
                          color: Colors.white,
                          fontWeight: FontWeight.w900,
                          fontSize: 16,
                          letterSpacing: 1.2,
                        ),
                      ),
                    ],
                  ),
                ),
              ),
              const SizedBox(height: 24),
              OutlinedButton.icon(
                style: OutlinedButton.styleFrom(
                  side: const BorderSide(color: Color(0xFF1CB0F6), width: 2),
                  shape: RoundedRectangleBorder(
                    borderRadius: BorderRadius.circular(16),
                  ),
                  padding: const EdgeInsets.symmetric(
                    horizontal: 24,
                    vertical: 14,
                  ),
                ),
                icon: const Icon(Icons.style, color: Color(0xFF1CB0F6)),
                label: const Text(
                  'УЧИТЬ КАРТОЧКИ СЛОВ',
                  style: TextStyle(
                    color: Color(0xFF1CB0F6),
                    fontWeight: FontWeight.bold,
                    fontSize: 16,
                  ),
                ),
                onPressed: () {
                  Navigator.push(
                    context,
                    MaterialPageRoute(builder: (context) => FlashcardScreen()),
                  );
                },
              ),
              const SizedBox(height: 40),
              Text(
                'Рады видеть тебя, ${UserProfile.userName}!',
                style: const TextStyle(
                  fontSize: 20,
                  fontWeight: FontWeight.bold,
                  color: Color(0xFF3C3C3C),
                ),
              ),
              const SizedBox(height: 8),
              Text(
                'Успешно пройдено сессий: ${UserProfile.completedLessons}',
                style: TextStyle(color: Colors.grey.shade600, fontSize: 16),
              ),
              if (UserProfile.doubleXpActive) ...[
                const SizedBox(height: 16),
                Container(
                  padding: const EdgeInsets.symmetric(
                    horizontal: 14,
                    vertical: 6,
                  ),
                  decoration: BoxDecoration(
                    color: Colors.orange,
                    borderRadius: BorderRadius.circular(20),
                  ),
                  child: const Text(
                    '🔥 Бустер Двойного XP активен!',
                    style: TextStyle(
                      color: Colors.white,
                      fontWeight: FontWeight.bold,
                    ),
                  ),
                ),
              ],
            ],
          ),
        ),
      ),
    );
  }
}

class LeaderboardScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    bool found = false;
    for (var u in UserProfile.leaderboard) {
      if (u['name'] == UserProfile.userName) {
        u['xp'] = UserProfile.totalXP;
        found = true;
      }
    }
    if (!found)
      UserProfile.leaderboard.add({
        'name': UserProfile.userName,
        'xp': UserProfile.totalXP,
      });
    UserProfile.leaderboard.sort(
      (a, b) => (b['xp'] as int).compareTo(a['xp'] as int),
    );

    return Scaffold(
      appBar: AppBar(
        title: const Text(
          'Таблица лидеров Лиги',
          style: TextStyle(
            color: Color(0xFF3C3C3C),
            fontWeight: FontWeight.bold,
          ),
        ),
        backgroundColor: Colors.white,
        elevation: 0,
        iconTheme: const IconThemeData(color: Color(0xFF3C3C3C)),
      ),
      body: Padding(
        padding: const EdgeInsets.all(16.0),
        child: ListView.builder(
          itemCount: UserProfile.leaderboard.length,
          itemBuilder: (context, index) {
            final user = UserProfile.leaderboard[index];
            bool isMe = user['name'] == UserProfile.userName;
            return Card(
              elevation: 0,
              margin: const EdgeInsets.symmetric(vertical: 6),
              shape: RoundedRectangleBorder(
                borderRadius: BorderRadius.circular(16),
                side: BorderSide(
                  color: isMe ? const Color(0xFF58CC02) : Colors.grey.shade200,
                  width: 2,
                ),
              ),
              color: isMe ? Colors.green.shade50 : Colors.grey.shade50,
              child: ListTile(
                leading: CircleAvatar(
                  backgroundColor: index == 0
                      ? Colors.amber
                      : (index == 1
                            ? Colors.grey.shade300
                            : Colors.orange.shade300),
                  child: Text(
                    '${index + 1}',
                    style: const TextStyle(
                      fontWeight: FontWeight.bold,
                      color: Colors.white,
                    ),
                  ),
                ),
                title: Text(
                  user['name'].toString(),
                  style: TextStyle(
                    fontWeight: isMe ? FontWeight.bold : FontWeight.normal,
                    fontSize: 18,
                    color: const Color(0xFF3C3C3C),
                  ),
                ),
                trailing: Text(
                  '${user['xp']} XP',
                  style: const TextStyle(
                    fontWeight: FontWeight.bold,
                    color: Colors.blueGrey,
                    fontSize: 16,
                  ),
                ),
              ),
            );
          },
        ),
      ),
    );
  }
}

class FlashcardScreen extends StatefulWidget {
  @override
  _FlashcardScreenState createState() => _FlashcardScreenState();
}

class _FlashcardScreenState extends State {
  final List _cards = [
    Flashcard(english: 'Education', russian: 'Образование'),
    Flashcard(english: 'Honestly', russian: 'Честно / Открыто'),
    Flashcard(english: 'Languages', russian: 'Языки'),
    Flashcard(english: 'Free', russian: 'Бесплатный / Свободный'),
    Flashcard(english: 'Delicious', russian: 'Вкусный / Восхитительный'),
    Flashcard(english: 'Understand', russian: 'Понимать'),
    Flashcard(english: 'Beautiful', russian: 'Красивый / Прекрасный'),
  ];
  int _currentIndex = 0;
  bool _showEnglish = true;
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text(
          'Интерактивные Карточки',
          style: TextStyle(
            color: Color(0xFF3C3C3C),
            fontWeight: FontWeight.bold,
          ),
        ),
        backgroundColor: Colors.white,
        elevation: 0,
        iconTheme: const IconThemeData(color: Color(0xFF3C3C3C)),
      ),
      body: Padding(
        padding: const EdgeInsets.all(24.0),
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            Text(
              'Карточка ${_currentIndex + 1} из ${_cards.length}',
              style: const TextStyle(
                color: Colors.grey,
                fontSize: 16,
                fontWeight: FontWeight.bold,
              ),
            ),
            const SizedBox(height: 24),
            GestureDetector(
              onTap: () {
                setState(() {
                  _showEnglish = !_showEnglish;
                });
              },
              child: Container(
                width: double.infinity,
                height: 240,
                decoration: BoxDecoration(
                  color: _showEnglish
                      ? const Color(0xFF1CB0F6)
                      : const Color(0xFF58CC02),
                  borderRadius: BorderRadius.circular(24),
                  boxShadow: [
                    BoxShadow(
                      color: Colors.grey.withOpacity(0.2),
                      blurRadius: 12,
                      offset: const Offset(0, 6),
                    ),
                  ],
                ),
                child: Center(
                  child: Padding(
                    padding: const EdgeInsets.all(16.0),
                    child: Text(
                      _showEnglish
                          ? _cards[_currentIndex].english
                          : _cards[_currentIndex].russian,
                      textAlign: TextAlign.center,
                      style: const TextStyle(
                        color: Colors.white,
                        fontSize: 32,
                        fontWeight: FontWeight.w900,
                        letterSpacing: 0.5,
                      ),
                    ),
                  ),
                ),
              ),
            ),
            const SizedBox(height: 12),
            const Text(
              '💡 Тапни по карточке, чтобы увидеть перевод!',
              style: TextStyle(color: Colors.grey, fontStyle: FontStyle.italic),
            ),
            const SizedBox(height: 48),
            Row(
              mainAxisAlignment: MainAxisAlignment.spaceEvenly,
              children: [
                ElevatedButton(
                  style: ElevatedButton.styleFrom(
                    backgroundColor: Colors.grey.shade200,
                    elevation: 0,
                  ),
                  onPressed: _currentIndex == 0
                      ? null
                      : () {
                          setState(() {
                            _currentIndex--;
                            _showEnglish = true;
                          });
                        },
                  child: const Text(
                    'НАЗАД',
                    style: TextStyle(color: Colors.black87),
                  ),
                ),
                ElevatedButton(
                  style: ElevatedButton.styleFrom(
                    backgroundColor: const Color(0xFF3C3C3C),
                    elevation: 0,
                  ),
                  onPressed: () {
                    setState(() {
                      if (_currentIndex < _cards.length - 1) {
                        _currentIndex++;
                        _showEnglish = true;
                      } else {
                        Navigator.pop(context);
                      }
                    });
                  },
                  child: Text(
                    _currentIndex == _cards.length - 1 ? 'ПОНЯТНО' : 'ДАЛЬШЕ',
                    style: const TextStyle(color: Colors.white),
                  ),
                ),
              ],
            ),
          ],
        ),
      ),
    );
  }
}

class ProfileScreen extends StatefulWidget {
  @override
  _ProfileScreenState createState() => _ProfileScreenState();
}

class _ProfileScreenState extends State {
  // Жестко привязал состояние к классу профиля
  final TextEditingController _nameController = TextEditingController();
  void _showChangeNameDialog() {
    _nameController.text = UserProfile.userName;
    showDialog(
      context: context,
      builder: (context) => AlertDialog(
        shape: RoundedRectangleBorder(borderRadius: BorderRadius.circular(16)),
        title: const Text(
          'Изменить имя профиля',
          style: TextStyle(fontWeight: FontWeight.bold),
        ),
        content: TextField(
          controller: _nameController,
          decoration: const InputDecoration(hintText: "Введите новый ник"),
          maxLength: 20,
        ),
        actions: [
          TextButton(
            onPressed: () => Navigator.pop(context),
            child: const Text('Отмена', style: TextStyle(color: Colors.grey)),
          ),
          ElevatedButton(
            style: ElevatedButton.styleFrom(
              backgroundColor: const Color(0xFF58CC02),
            ),
            onPressed: () {
              if (_nameController.text.trim().isNotEmpty) {
                setState(() {
                  UserProfile.userName = _nameController.text.trim();
                });
                Navigator.pop(context);
              }
            },
            child: const Text(
              'Сохранить',
              style: TextStyle(color: Colors.white),
            ),
          ),
        ],
      ),
    );
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text(
          'Мой Профиль',
          style: TextStyle(
            color: Color(0xFF3C3C3C),
            fontWeight: FontWeight.bold,
          ),
        ),
        backgroundColor: Colors.white,
        elevation: 0,
      ),
      body: Padding(
        padding: const EdgeInsets.all(24.0),
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.start,
          children: [
            Container(
              padding: const EdgeInsets.all(16),
              decoration: BoxDecoration(
                color: Colors.grey.shade50,
                borderRadius: BorderRadius.circular(20),
                border: Border.all(color: Colors.grey.shade200, width: 2),
              ),
              child: Row(
                children: [
                  CircleAvatar(
                    radius: 36,
                    backgroundColor: Colors.green.shade50,
                    child: const Text('👑', style: TextStyle(fontSize: 36)),
                  ),
                  const SizedBox(width: 16),
                  Expanded(
                    child: Column(
                      crossAxisAlignment: CrossAxisAlignment.start,
                      children: [
                        Text(
                          UserProfile.userName,
                          style: const TextStyle(
                            fontSize: 22,
                            fontWeight: FontWeight.w900,
                            color: Color(0xFF3C3C3C),
                          ),
                        ),
                        const SizedBox(height: 4),
                        Text(
                          'Звание: Ранг ${UserProfile.currentLevel}',
                          style: const TextStyle(
                            fontSize: 16,
                            color: Color(0xFF58CC02),
                            fontWeight: FontWeight.bold,
                          ),
                        ),
                      ],
                    ),
                  ),
                  IconButton(
                    icon: const Icon(Icons.edit, color: Color(0xFF58CC02)),
                    onPressed: _showChangeNameDialog,
                  ),
                ],
              ),
            ),
            const SizedBox(height: 32),
            const Text(
              'Статистика без обмана',
              style: TextStyle(
                fontSize: 18,
                fontWeight: FontWeight.bold,
                color: Color(0xFF3C3C3C),
              ),
            ),
            const SizedBox(height: 16),
            Row(
              children: [
                Expanded(
                  child: Card(
                    elevation: 0,
                    shape: RoundedRectangleBorder(
                      borderRadius: BorderRadius.circular(16),
                      side: BorderSide(color: Colors.grey.shade200, width: 2),
                    ),
                    child: Padding(
                      padding: const EdgeInsets.all(16.0),
                      child: Column(
                        children: [
                          Text(
                            '${UserProfile.totalXP}',
                            style: const TextStyle(
                              fontSize: 26,
                              fontWeight: FontWeight.w900,
                              color: Colors.orange,
                            ),
                          ),
                          const SizedBox(height: 4),
                          const Text(
                            'Очки XP',
                            style: TextStyle(
                              color: Colors.grey,
                              fontWeight: FontWeight.bold,
                            ),
                          ),
                        ],
                      ),
                    ),
                  ),
                ),
                const SizedBox(width: 16),
                Expanded(
                  child: Card(
                    elevation: 0,
                    shape: RoundedRectangleBorder(
                      borderRadius: BorderRadius.circular(16),
                      side: BorderSide(color: Colors.grey.shade200, width: 2),
                    ),
                    child: Padding(
                      padding: const EdgeInsets.all(16.0),
                      child: Column(
                        children: [
                          Text(
                            '${UserProfile.completedLessons}',
                            style: const TextStyle(
                              fontSize: 26,
                              fontWeight: FontWeight.w900,
                              color: Color(0xFF58CC02),
                            ),
                          ),
                          const SizedBox(height: 4),
                          const Text(
                            'Уроки',
                            style: TextStyle(
                              color: Colors.grey,
                              fontWeight: FontWeight.bold,
                            ),
                          ),
                        ],
                      ),
                    ),
                  ),
                ),
              ],
            ),
          ],
        ),
      ),
    );
  }
}

class ShopScreen extends StatefulWidget {
  @override
  _ShopScreenState createState() => _ShopScreenState();
}

class _ShopScreenState extends State {
  void _buyItem(
    BuildContext context,
    String name,
    int cost,
    VoidCallback action,
  ) {
    if (UserProfile.totalXP >= cost) {
      setState(() {
        UserProfile.totalXP -= cost;
        action();
      });
      ScaffoldMessenger.of(
        context,
      ).showSnackBar(SnackBar(content: Text('🎉 Вы успешно купили: $name!')));
    } else {
      ScaffoldMessenger.of(context).showSnackBar(
        const SnackBar(
          content: Text('❌ Недостаточно очков XP! Проходи тесты.'),
        ),
      );
    }
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text(
          'Магазин бонусов',
          style: TextStyle(
            color: Color(0xFF3C3C3C),
            fontWeight: FontWeight.bold,
          ),
        ),
        backgroundColor: Colors.white,
        elevation: 0,
      ),
      body: Padding(
        padding: const EdgeInsets.all(24.0),
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.start,
          children: [
            Text(
              'Баланс: ${UserProfile.totalXP} XP',
              style: const TextStyle(
                fontSize: 20,
                fontWeight: FontWeight.bold,
                color: Colors.orange,
              ),
            ),
            const SizedBox(height: 24),
            Card(
              shape: RoundedRectangleBorder(
                borderRadius: BorderRadius.circular(16),
                side: BorderSide(color: Colors.grey.shade200, width: 2),
              ),
              child: ListTile(
                leading: const Text('❄️', style: TextStyle(fontSize: 32)),
                title: const Text(
                  'Заморозка стрика',
                  style: TextStyle(fontWeight: FontWeight.bold),
                ),
                subtitle: Text('В наличии: ${UserProfile.streakFreezes} шт.'),
                trailing: ElevatedButton(
                  style: ElevatedButton.styleFrom(
                    backgroundColor: const Color(0xFF1CB0F6),
                  ),
                  onPressed: () => _buyItem(
                    context,
                    'Заморозка стрика',
                    50,
                    () => UserProfile.streakFreezes++,
                  ),
                  child: const Text(
                    '50 XP',
                    style: TextStyle(color: Colors.white),
                  ),
                ),
              ),
            ),
            const SizedBox(height: 16),
            Card(
              shape: RoundedRectangleBorder(
                borderRadius: BorderRadius.circular(16),
                side: BorderSide(color: Colors.grey.shade200, width: 2),
              ),
              child: ListTile(
                leading: const Text('🔥', style: TextStyle(fontSize: 32)),
                title: const Text(
                  'Двойной опыт',
                  style: TextStyle(fontWeight: FontWeight.bold),
                ),
                subtitle: Text(
                  UserProfile.doubleXpActive
                      ? 'Уже активирован'
                      : 'Удваивает XP за ответы',
                ),
                trailing: ElevatedButton(
                  style: ElevatedButton.styleFrom(
                    backgroundColor: const Color(0xFF58CC02),
                  ),
                  onPressed: UserProfile.doubleXpActive
                      ? null
                      : () => _buyItem(
                          context,
                          'Двойной опыт',
                          100,
                          () => UserProfile.doubleXpActive = true,
                        ),
                  child: const Text(
                    '100 XP',
                    style: TextStyle(color: Colors.white),
                  ),
                ),
              ),
            ),
          ],
        ),
      ),
    );
  }
}

class LessonScreen extends StatefulWidget {
  @override
  _LessonScreenState createState() => _LessonScreenState();
}

class _LessonScreenState extends State {
  final List _sourceQuestions = [
    Task(
      russianText: '«Привет, я не использую Дуолинго»',
      correctOrder: ['Hello', 'I', 'do', 'not', 'use', 'Duolingo'],
      availableWords: ['not', 'Hello', 'Duolingo', 'am', 'I', 'use', 'do'],
    ),
    Task(
      russianText: '«Я хочу учить языки честно»',
      correctOrder: ['I', 'want', 'to', 'learn', 'languages', 'honestly'],
      availableWords: [
        'honestly',
        'to',
        'languages',
        'badly',
        'I',
        'learn',
        'want',
      ],
    ),
    Task(
      russianText: '«Образование должно быть бесплатным»',
      correctOrder: ['Education', 'must', 'be', 'free'],
      availableWords: ['free', 'expensive', 'must', 'be', 'Education', 'pay'],
    ),
    Task(
      russianText: '«Я хочу заказать чашку кофе»',
      correctOrder: ['I', 'want', 'to', 'order', 'a', 'cup', 'of', 'coffee'],
      availableWords: [
        'want',
        'coffee',
        'order',
        'cup',
        'I',
        'to',
        'a',
        'of',
        'tea',
      ],
    ),
    Task(
      russianText: '«Где находится ближайший отель?»',
      correctOrder: ['Where', 'is', 'the', 'nearest', 'hotel'],
      availableWords: [
        'nearest',
        'hotel',
        'Where',
        'is',
        'the',
        'shop',
        'station',
      ],
    ),
    Task(
      russianText: '«Я изучаю английский язык каждый день»',
      correctOrder: ['I', 'study', 'English', 'every', 'day'],
      availableWords: ['English', 'study', 'every', 'I', 'day', 'week', 'know'],
    ),
    Task(
      russianText: '«Приятно познакомиться с вами»',
      correctOrder: ['Nice', 'to', 'meet', 'you'],
      availableWords: ['meet', 'Nice', 'you', 'to', 'see', 'good'],
    ),
    Task(
      russianText: '«Сколько стоит этот билет?»',
      correctOrder: ['How', 'much', 'is', 'this', 'ticket'],
      availableWords: ['much', 'ticket', 'is', 'How', 'this', 'cost', 'that'],
    ),
    Task(
      russianText: '«Вы можете мне помочь?»',
      correctOrder: ['Can', 'you', 'help', 'me'],
      availableWords: ['help', 'Can', 'me', 'you', 'do', 'show'],
    ),
    Task(
      russianText: '«Мне нужен счет, пожалуйста»',
      correctOrder: ['I', 'need', 'the', 'bill', 'please'],
      availableWords: ['bill', 'please', 'need', 'I', 'the', 'menu', 'food'],
    ),
  ];
  final List _sessionQuestions = [];
  int _currentTaskIndex = 0;
  List _selectedWords = [];
  List _currentAvailableWords = [];
  String _feedbackMessage = '';
  Color _feedbackColor = Colors.transparent;
  bool _isCorrect = false;
  @override
  void initState() {
    super.initState();
    List giantPool = [];
    for (int i = 0; i < 400; i++) {
      var base = _sourceQuestions[i % _sourceQuestions.length];
      giantPool.add(
        Task(
          russianText: '${base.russianText} (Урок ${i + 1})',
          correctOrder: base.correctOrder,
          availableWords: base.availableWords,
        ),
      );
    }
    int startOffset = (UserProfile.completedLessons * 7) % 390;
    for (int j = 0; j < 7; j++) {
      _sessionQuestions.add(giantPool[startOffset + j]);
    }
    _loadTask();
  }

  void _loadTask() {
    _selectedWords = [];
    _currentAvailableWords = List.from(
      _sessionQuestions[_currentTaskIndex].availableWords,
    );
    _feedbackMessage = '';
    _feedbackColor = Colors.transparent;
    _isCorrect = false;
  }

  void _checkAnswer() {
    final currentTask = _sessionQuestions[_currentTaskIndex];
    setState(() {
      if (_selectedWords.length == currentTask.correctOrder.length &&
          List.generate(
            currentTask.correctOrder.length,
            (i) => _selectedWords[i] == currentTask.correctOrder[i],
          ).every((e) => e)) {
        _feedbackMessage = '🎉 Потрясающе! Ответ верный!';
        _feedbackColor = const Color(0xFF58CC02);
        _isCorrect = true;
        UserProfile.addXP(15);
      } else {
        _feedbackMessage = '❌ Ошибка в порядке слов!';
        _feedbackColor = const Color(0xFFEA2B2B);
        _isCorrect = false;
      }
    });
  }

  void _nextStep() {
    setState(() {
      if (_currentTaskIndex < _sessionQuestions.length - 1) {
        _currentTaskIndex++;
        _loadTask();
      } else {
        UserProfile.completedLessons += 1;
        Navigator.pushReplacement(
          context,
          MaterialPageRoute(builder: (context) => VictoryScreen()),
        );
      }
    });
  }

  @override
  Widget build(BuildContext context) {
    final currentTask = _sessionQuestions[_currentTaskIndex];
    double progress =
        (_currentTaskIndex + (_isCorrect ? 1.0 : 0.0)) /
        _sessionQuestions.length;
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(
        title: Text(
          'Шаг ${_currentTaskIndex + 1} из ${_sessionQuestions.length}',
          style: const TextStyle(
            color: Color(0xFF3C3C3C),
            fontWeight: FontWeight.bold,
          ),
        ),
        backgroundColor: Colors.white,
        elevation: 0,
        iconTheme: const IconThemeData(color: Color(0xFF3C3C3C)),
      ),
      body: Padding(
        padding: const EdgeInsets.all(24.0),
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.start,
          children: [
            ClipRRect(
              borderRadius: BorderRadius.circular(8),
              child: LinearProgressIndicator(
                value: progress,
                backgroundColor: Colors.grey.shade100,
                valueColor: const AlwaysStoppedAnimation(Color(0xFF58CC02)),
                minHeight: 12,
              ),
            ),
            const SizedBox(height: 32),
            const Text(
              'Переведи это предложение:',
              style: TextStyle(
                fontSize: 22,
                fontWeight: FontWeight.w900,
                color: Color(0xFF3C3C3C),
              ),
            ),
            const SizedBox(height: 12),
            Container(
              padding: const EdgeInsets.all(16),
              decoration: BoxDecoration(
                color: Colors.grey.shade50,
                borderRadius: BorderRadius.circular(16),
              ),
              child: Row(
                children: [
                  const Text('🦉', style: TextStyle(fontSize: 28)),
                  const SizedBox(width: 12),
                  Expanded(
                    child: Text(
                      currentTask.russianText,
                      style: const TextStyle(
                        fontSize: 18,
                        color: Color(0xFF3C3C3C),
                        fontWeight: FontWeight.w500,
                      ),
                    ),
                  ),
                ],
              ),
            ),
            const SizedBox(height: 32),
            Container(
              constraints: const BoxConstraints(minHeight: 80),
              width: double.infinity,
              decoration: BoxDecoration(
                border: Border(
                  bottom: BorderSide(color: Colors.grey.shade200, width: 3),
                ),
              ),
              child: Wrap(
                spacing: 8,
                runSpacing: 8,
                children: _selectedWords
                    .map(
                      (word) => OutlinedButton(
                        style: OutlinedButton.styleFrom(
                          side: BorderSide(
                            color: Colors.grey.shade300,
                            width: 2,
                          ),
                          shape: RoundedRectangleBorder(
                            borderRadius: BorderRadius.circular(12),
                          ),
                          padding: const EdgeInsets.symmetric(
                            horizontal: 16,
                            vertical: 12,
                          ),
                        ),
                        onPressed: _isCorrect
                            ? null
                            : () {
                                setState(() {
                                  _selectedWords.remove(word);
                                  _currentAvailableWords.add(word);
                                });
                              },
                        child: Text(
                          word,
                          style: const TextStyle(
                            fontSize: 16,
                            color: Color(0xFF3C3C3C),
                            fontWeight: FontWeight.bold,
                          ),
                        ),
                      ),
                    )
                    .toList(),
              ),
            ),
            const SizedBox(height: 32),
            Wrap(
              spacing: 10,
              runSpacing: 10,
              children: _currentAvailableWords
                  .map(
                    (word) => ElevatedButton(
                      style: ElevatedButton.styleFrom(
                        backgroundColor: Colors.white,
                        foregroundColor: const Color(0xFF3C3C3C),
                        elevation: 2,
                        shadowColor: Colors.grey.shade300,
                        side: BorderSide(color: Colors.grey.shade200, width: 2),
                        shape: RoundedRectangleBorder(
                          borderRadius: BorderRadius.circular(14),
                        ),
                        padding: const EdgeInsets.symmetric(
                          horizontal: 20,
                          vertical: 14,
                        ),
                      ),
                      onPressed: _isCorrect
                          ? null
                          : () {
                              setState(() {
                                _selectedWords.add(word);
                                _currentAvailableWords.remove(word);
                              });
                            },
                      child: Text(
                        word,
                        style: const TextStyle(
                          fontSize: 16,
                          fontWeight: FontWeight.bold,
                        ),
                      ),
                    ),
                  )
                  .toList(),
            ),
            const Spacer(),
            Center(
              child: Text(
                _feedbackMessage,
                style: TextStyle(
                  fontSize: 18,
                  color: _feedbackColor,
                  fontWeight: FontWeight.w900,
                ),
              ),
            ),
            const SizedBox(height: 16),
            SizedBox(
              width: double.infinity,
              height: 58,
              child: ElevatedButton(
                style: ElevatedButton.styleFrom(
                  backgroundColor: _isCorrect
                      ? const Color(0xFF58CC02)
                      : const Color(0xFF1CB0F6),
                  shape: RoundedRectangleBorder(
                    borderRadius: BorderRadius.circular(16),
                  ),
                  elevation: 0,
                ),
                onPressed: _selectedWords.isEmpty
                    ? null
                    : (_isCorrect ? _nextStep : _checkAnswer),
                child: Text(
                  _isCorrect ? 'ПРОДОЛЖИТЬ' : 'ПРОВЕРИТЬ ОТВЕТ',
                  style: const TextStyle(
                    color: Colors.white,
                    fontSize: 18,
                    fontWeight: FontWeight.w900,
                    letterSpacing: 0.5,
                  ),
                ),
              ),
            ),
          ],
        ),
      ),
    );
  }
}

class VictoryScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: SafeArea(
        child: Padding(
          padding: const EdgeInsets.all(32.0),
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
            children: [
              const Text('🎉🏆👑', style: TextStyle(fontSize: 70)),
              const SizedBox(height: 24),
              const Text(
                'Идеальный урок!',
                style: TextStyle(
                  fontSize: 28,
                  fontWeight: FontWeight.w900,
                  color: Color(0xFF58CC02),
                ),
              ),
              const SizedBox(height: 16),
              Text(
                'Сессия из 7 заданий успешно завершена. Очки зачислены, а твой ранг в таблице лидеров вырос! Продолжай в том же духе.',
                textAlign: TextAlign.center,
                style: const TextStyle(
                  fontSize: 16,
                  color: Colors.grey,
                  height: 1.4,
                ),
              ),
              const SizedBox(height: 48),
              SizedBox(
                width: double.infinity,
                height: 56,
                child: ElevatedButton(
                  style: ElevatedButton.styleFrom(
                    backgroundColor: const Color(0xFF3C3C3C),
                    shape: RoundedRectangleBorder(
                      borderRadius: BorderRadius.circular(16),
                    ),
                    elevation: 0,
                  ),
                  onPressed: () {
                    Navigator.popUntil(context, (route) => route.isFirst);
                  },
                  child: const Text(
                    'В ГЛАВНОЕ МЕНЮ',
                    style: TextStyle(
                      color: Colors.white,
                      fontSize: 18,
                      fontWeight: FontWeight.bold,
                    ),
                  ),
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
