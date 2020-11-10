---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8430fb8935d0e14cbee6114490b95203edc97a5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979330"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageRuleCollectionPage messageRules = graphClient.me().mailFolders("inbox").messageRules()
    .buildRequest()
    .get();

```