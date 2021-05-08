---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1c0d24514a2490fc8eb9b7dcdbe9ca693c752c0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var settings = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Settings
    .Request()
    .GetAsync();

```