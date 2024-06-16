# Microsoft-Wizards


'서비스(Services)'나 '에이전트(Agents)'라는 용어를 사용합니다. 이들은 백그라운드에서 실행되며 사용자와 직접적인 상호작용 없이 특정 작업을 수행하는 프로그램입니다.

1. 서비스(Services):
- 시스템 부팅 시 자동으로 시작되며, 지속적으로 실행됩니다.
- 시스템 전반에 걸쳐 필요한 기능을 제공하며, 다른 프로세스나 애플리케이션에 서비스를 제공합니다.
- `/System/Library/LaunchDaemons` 또는 `/Library/LaunchDaemons` 디렉토리에 plist 파일로 정의됩니다.

2. 에이전트(Agents):
- 사용자 로그인 시 시작되며, 사용자별로 실행됩니다.
- 특정 사용자와 관련된 작업을 수행하며, 해당 사용자의 컨텍스트에서 실행됩니다.
- `/System/Library/LaunchAgents`, `/Library/LaunchAgents` 또는 `~/Library/LaunchAgents` 디렉토리에 plist 파일로 정의됩니다.

이러한 서비스와 에이전트는 launchd라는 프로세스 관리자에 의해 관리되고 실행됩니다. launchd는 시스템 부팅 시 필요한 프로세스를 자동으로 시작하고, 필요에 따라 프로세스를 종료하거나 재시작하는 역할을 합니다.

윈도우에서의 서비스(Services)는 맥에서의 서비스와 유사한 개념으로, 백그라운드에서 실행되며 시스템 기능을 제공합니다. 윈도우의 서비스 제어 관리자(SCM)가 launchd와 비슷한 역할을 수행합니다.
