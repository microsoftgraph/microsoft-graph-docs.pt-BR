---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1765351c4351c1c71b4d434de335455ec8443aadd9ceeb54842d4edc2f468f5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099367"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingAttendanceReport meetingAttendanceReport = graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy").meetingAttendanceReport()
    .buildRequest()
    .get();

```