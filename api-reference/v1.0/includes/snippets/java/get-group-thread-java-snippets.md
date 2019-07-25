---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99207124d04764137f40e362c92f85f6ce2b3f17
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889387"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThread conversationThread = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").threads("AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==")
    .buildRequest()
    .get();

```