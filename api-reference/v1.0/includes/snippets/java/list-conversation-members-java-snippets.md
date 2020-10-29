---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aea1f1e15ac659b3c29fcdd768e95c4f87e2a5b1
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782982"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content members = graphClient.me().chats().{id}().members()
    .buildRequest()
    .get();

```