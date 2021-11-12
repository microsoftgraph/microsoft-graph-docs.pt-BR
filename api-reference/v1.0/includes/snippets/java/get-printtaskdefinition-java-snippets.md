---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 469d2962e70d5b555657bfa2a1e8c765f7965e9aa7fb28f26266cb3b21abfbf2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271992"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskDefinition printTaskDefinition = graphClient.print().taskDefinitions("{printTaskDefinitionId}")
    .buildRequest()
    .get();

```