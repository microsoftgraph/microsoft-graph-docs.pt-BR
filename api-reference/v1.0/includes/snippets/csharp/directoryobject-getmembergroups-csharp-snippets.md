---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03fff4d63aa4237b7b3993b5805ea9fbd0296bc1
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```