---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be3aee44ad43baf12abc0fa24b2f5aab88311751
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873858"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMemberOf = await graphClient.Me.ScopedRoleMemberOf
    .Request()
    .GetAsync();

```