---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0f5ac7ae03d2b92ec69e3a7d417c4d28af810d41
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081022"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["{teamsId}"].Members
    .Request()
    .GetAsync();

```