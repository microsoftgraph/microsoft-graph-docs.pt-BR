---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae99f4133727fca5ffa870faf55ea9f0a5d3ef8e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123542"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalMeetingRegistration meetingRegistration = new ExternalMeetingRegistration();
meetingRegistration.allowedRegistrant = MeetingAudience.EVERYONE;

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration()
    .buildRequest()
    .post(meetingRegistration);

```