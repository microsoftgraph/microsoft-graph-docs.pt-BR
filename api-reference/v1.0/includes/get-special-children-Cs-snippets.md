---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 130de052d6f9e09a2f89001353900cf754bdfa06
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Special["{special-folder-name}"].Children
    .Request()
    .GetAsync();

```