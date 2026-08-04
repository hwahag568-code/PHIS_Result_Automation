# PHIS Result Automation 배포

이 저장소는 PHIS Result Automation의 **설치파일 배포 전용** 공개
저장소입니다. 소스 코드, 실제 배포 설정, 로그 및 검사 데이터는 공개하지
않습니다.

최신 설치파일은 [Latest Release](https://github.com/hwahag568-code/PHIS_Result_Automation/releases/latest)에서
받을 수 있습니다. 설치된 프로그램은 실행 시 새 Release를 자동으로 확인하며,
PHIS 작업 중에 확인된 업데이트는 작업이 끝난 뒤 처리합니다. GUI에는 수동
업데이트 확인 버튼이나 마지막 확인 시각을 표시하지 않습니다.

신규 설치와 수동 복구에는 Release의
`PHIS_Result_Automation_Setup_<버전>.exe` 전체 설치파일을 사용합니다.
자동 업데이트는 현재 설치본과 호환되는 같은 런타임 세대의 경량 패치가
있으면 작은 `PHIS_Result_Automation_Update_<세대>_<버전>.exe`를 우선
사용하고, 패치가 없거나 런타임 세대가 다르면 전체 설치파일로 자동
전환합니다. 경량 업데이트 지원 이전 버전에서는 먼저 전체 설치파일로
지원 버전을 한 번 설치해야 하며, 이후 같은 런타임 세대의 업데이트부터
경량 패치를 사용할 수 있습니다.

각 Release의 태그와 설치파일 이름은 버전마다 고유합니다. 이미 공개한
Release 파일을 같은 태그로 교체하지 않으며, 수정본은 새 버전으로
배포합니다. 전체 설치파일은 항상 제공하며, 각 Release에는 런타임 세대와
자산 구성을 기록한 manifest도 함께 제공합니다.

이 프로그램은 허가된 업무 환경에서만 사용해야 합니다. 설치파일에
코드서명이 적용되지 않은 배포에서는 Windows 보안 경고가 표시될 수 있습니다.
