---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d42e04773f7b2d9443faee24fe4b2ca9d298ba65
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953652"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

UUID onBehalfOfUserId = UUID.fromString("onBehalfOfUserId-value");

graphClient.groups("{id}")
    .validateProperties(displayName,mailNickname,onBehalfOfUserId)
    .buildRequest()
    .post();

```