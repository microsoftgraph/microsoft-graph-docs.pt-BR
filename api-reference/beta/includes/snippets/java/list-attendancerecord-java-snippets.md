---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5ef483719e6f5d17046b3c0c3b23af829b81a86
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223572"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttendanceRecordCollectionPage attendanceRecords = graphClient.me().onlineMeetings("{meetingId}").attendanceReports("{reportId}").attendanceRecords()
    .buildRequest()
    .get();

```