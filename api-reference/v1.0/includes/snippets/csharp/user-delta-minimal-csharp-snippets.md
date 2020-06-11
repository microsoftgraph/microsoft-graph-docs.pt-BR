---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a111b8dd47f7be928342ce54b58c300274d1bdd9
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users
    .Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select("displayName,jobTitle,mobilePhone")
    .GetAsync();

```