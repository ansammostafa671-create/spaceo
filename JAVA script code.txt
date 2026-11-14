let currentMission = 1;

function showScreen(screenId) {
    // إخفاء كل الشاشات
    const screens = document.querySelectorAll('.screen');
    screens.forEach(screen => screen.classList.remove('active'));
    
    // إظهار الشاشة المطلوبة فقط
    document.getElementById(screenId).classList.add('active');
}

function startMission(missionNum) {
    currentMission = missionNum;
    document.getElementById('active-mission-label').innerText = `MISSION 03: ASSEMBLY`;
    showScreen('assembly-screen');
}

function selectComponent(name, mass, cost) {
    console.log(`Selected: ${name}, Mass: ${mass}, Cost: ${cost}`);
    // هنا بيتم تحديث المتغيرات بتاعت الميزانية والوزن برمجياً
}