---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 272ae40f8fb5373e7e02cd3b85a783cc2211fe67
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713365"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entityType = "Group";

var displayName = "Myprefix_test_mysuffix";

var mailNickname = "Myprefix_test_mysuffix";

var onBehalfOfUserId = "onBehalfOfUserId-value";

await graphClient.DirectoryObjects
    .ValidateProperties(entityType,displayName,mailNickname,onBehalfOfUserId)
    .Request()
    .PostAsync();

```