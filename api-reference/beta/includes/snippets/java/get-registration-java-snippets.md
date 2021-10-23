---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bef15d02c70aba34c44c30b49e8f27d5c3747aa5
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistration meetingRegistration = graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration()
    .buildRequest()
    .expand("customQuestions")
    .get();

```