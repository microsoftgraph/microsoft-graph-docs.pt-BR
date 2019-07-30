---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 272ae40f8fb5373e7e02cd3b85a783cc2211fe67
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932196"
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