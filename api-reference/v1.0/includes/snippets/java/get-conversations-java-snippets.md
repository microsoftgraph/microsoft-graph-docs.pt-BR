---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0840e43496616f76e0c6ba2450a6a035b3b9aea5eff96fe515eeb42f91fe9dec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273461"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationCollectionPage conversations = graphClient.groups("{id}").conversations()
    .buildRequest()
    .get();

```