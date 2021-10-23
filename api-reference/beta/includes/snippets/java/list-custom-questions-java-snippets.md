---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfb97a0640b957215f5ff49cd8522f2b0abe4d2f
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561220"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistrationQuestionCollectionPage customQuestions = graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().customQuestions()
    .buildRequest()
    .get();

```