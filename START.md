# Запуск minibus для Санкт-Петербурга

Запуск 10 % от population.xml

`<removePercentOfPopulation(scenario.getPopulation(), 90);>` 

config.xml взят из сетки 4 на 4 из статьи Неймана.
оригинальный конфиг - config_original.xml
    
Изменения:
    
    `<param name="earningsPerBoardingPassenger" value="100.0" /> <!--1.0-->`
    
    <param name="minX" value="676000.0" />
    <param name="maxX" value="688000.0" />
    <param name="minY" value="6636000.0" />
    <param name="maxY" value="6646000.0" />
    
    <param name="activityType_1"            value="e" />
    <param name="activityPriority_1"        value="1" />
    <param name="activityTypicalDuration_1" value="06:00:00" />
    <param name="activityMinimalDuration_1" value="02:00:00" />

    <param name="activityType_2"            value="w" />
    <param name="activityPriority_2"        value="1" />
    <param name="activityTypicalDuration_2" value="08:00:00" />
    <param name="activityMinimalDuration_2" value="06:00:00" />

    <param name="activityType_3"            value="s" />
    <param name="activityPriority_3"        value="1" />
    <param name="activityTypicalDuration_3" value="01:00:00" />
    <param name="activityMinimalDuration_3" value="00:10:00" />`
    
Результат: на нулевой итерации создаётся 2 остановок, которые не меняются в течение всех 100 итераций.
10 операторов работают на этих двух остановках.

