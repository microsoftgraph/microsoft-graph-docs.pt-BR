---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 130de052d6f9e09a2f89001353900cf754bdfa06
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Special["{special-folder-name}"].Children
    .Request()
    .GetAsync();

```