---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25cc4022c6edc1370ec56e03cdccf4a3bfcbe95d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210254"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedGroupSourceCollectionPage unifiedGroupSources = graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").unifiedGroupSources()
    .buildRequest()
    .get();

```