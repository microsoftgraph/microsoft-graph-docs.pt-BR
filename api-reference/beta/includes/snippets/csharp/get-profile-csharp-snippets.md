---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5a7ae4b8f6b95020104c6b25a8b6c14dc0cf7db4
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821157"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profile = await graphClient.Me.Profile
    .Request()
    .Expand("skills($select=displayName)")
    .GetAsync();

```