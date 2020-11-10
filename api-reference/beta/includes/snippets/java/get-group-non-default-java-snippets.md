---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07bfaba11be1239f4827dc3997d3c47e4c93a642
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965254"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.groups("b320ee12-b1cd-4cca-b648-a437be61c5cd")
    .buildRequest()
    .select("allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount")
    .get();

```