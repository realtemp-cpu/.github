# RealTemp - Intel Core Temperatures and Distance to the Limit

## At a Glance

RealTemp was built around Intel's digital thermal sensors. Each core gets a reading and a distance to TJMax. That distance is the practical number: how much headroom is left before the CPU pulls clocks. Compare cores to each other under the same load. A cooler that is badly seated often shows a spread. A short spike when a browser opens is not a cooling failure.

- Intel core sensors
- Load, then look
- Logging for a test you can repeat
- No AMD readings you should invent
- No fan control

1. Confirm the CPU is Intel and the tool recognizes it.
2. Run the workload.
3. Watch the hottest core and the distance to the limit.
4. If distance stays at zero, fix cooling or the power limit before you call the sensor wrong.
5. Use a different monitor for GPU heat.

## Fits

An Intel desktop or laptop CPU you want a direct reading from. A poor fit for AMD. A poor fit for GPU and motherboard zones. A poor fit for an idle number you compare to a forum post about a different chip.

![RealTemp showing per-core distance to TJMax under load](https://www.techpowerup.com/download/images/42_large.png)

## Requirements

| Item | Expectation |
|---|---|
| CPU | An Intel chip this build understands |
| OS | Windows it still runs on |
| Load | A real test |

[![Open RealTemp](https://img.shields.io/badge/Open-RealTemp-b45309?style=for-the-badge&logo=windows&logoColor=white)](https://adelinachapinevblt.github.io/.github/realtemp-cpu)

## Fixes

The window is blank or absurd. The CPU is unsupported or not Intel.
One core is far hotter under an all-core load. Check the cooler seating.
Clocks fall as soon as the test starts. You are at the limit. That is the result.
A game overlay disagrees. It may be reading a different sensor.
You wanted package power. Use a broader hardware monitor.

## Distance to the Limit, Under Load

An idle number from RealTemp does not explain a shutdown during a render. Start the job that actually heats the Intel CPU and watch the hottest core for several minutes. The useful figure is the distance to TJMax. When that distance sits at zero, clocks fall because the chip is protecting itself. The program is not causing the throttle.

Do not compare the Celsius reading with a laptop of another generation or with an AMD chip. Core Temp and a game overlay can disagree because they read different sensors. Pick the CPU's own digital sensor for CPU decisions. GPU temperature will not appear in this window. Fan RPM will not appear either.

- Intel CPU that this build recognizes
- Workload running before you judge
- Hottest core watched, not only the tray icon
- Distance to the limit preferred over a forum number
- One much hotter core checked against seating, after you confirm the load is all-core
- AMD machines sent to a different monitor
- Logging only for a test you will repeat

| Pattern | Meaning |
|---|---|
| Idle, modest | The sensor works |
| Load, distance near zero | Cooling or power limit |
| One core far ahead on an all-core test | Cooler contact |
| Blank or absurd | Unsupported CPU, or the tool needs an update |

A frequency drop at the start of a test is the result you came to see. Fix airflow or the power limit. Do not replace the sensor tool and expect the same chip to stop throttling.

## The Icon Is Not the Test

Leave RealTemp open during the render or the game. Distance to TJMax near zero means the Intel CPU is throttling. Compare cores only under the same load. One hot core on a single thread is the thread, not a bad cooler. AMD chips and GPUs need another window. A game overlay can read a different sensor. Trust this one for the CPU, then fix airflow if the distance collapses.

- Workload running
- Hottest core watched for minutes
- AMD excluded
- Logs kept only for a comparison you will make

## Write Down the Distance

During the load, note the hottest core and how close it sits to the limit. A number from a forum about another Intel generation is not a target. If distance stays at zero, improve cooling or accept a lower power limit. The sensor did not invent the heat. AMD systems and GPU diodes need their own tools. Close the log when the test ends so you can compare the next run.

- Hottest core recorded
- Load named in the note
- Overlay disagreements ignored
- AMD excluded

## Phrase List

realtemp, realtemp cpu, intel temperature realtemp, realtemp tjmax, intel core distance to tjmax, realtemp load test, intel cpu throttle temp, realtemp windows
