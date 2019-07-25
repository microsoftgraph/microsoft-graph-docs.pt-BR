---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b249f129d0cfad1de47396fc88e030a5cb591821
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "Myprefix_test_mysuffix";

var mailNickname = "Myprefix_test_mysuffix";

var onBehalfOfUserId = "onBehalfOfUserId-value";

await graphClient.Groups["{id}"]
    .ValidateProperties(displayName,mailNickname,onBehalfOfUserId)
    .Request()
    .PostAsync();

```