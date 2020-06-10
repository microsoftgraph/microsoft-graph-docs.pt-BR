---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 630d3679346d27b39f9a5e667eb32d1239a35754
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684362"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Contacts
    .Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select("displayName,jobTitle,mail")
    .GetAsync();

```