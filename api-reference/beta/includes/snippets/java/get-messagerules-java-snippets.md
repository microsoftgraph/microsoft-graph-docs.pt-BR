---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8430fb8935d0e14cbee6114490b95203edc97a5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879935"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageRuleCollectionPage messageRules = graphClient.me().mailFolders("inbox").messageRules()
    .buildRequest()
    .get();

```