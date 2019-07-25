---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddb37bbd59a0160ea75c8691cf2424ec60fdfb43
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895319"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.chats("{id}").messages("{id}")
    .buildRequest()
    .get();

```