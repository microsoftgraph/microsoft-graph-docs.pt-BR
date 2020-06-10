---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b581dd6d2df13d55af63356067072d5a5392508d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684180"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var response = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails["{thumb-id}"]["{size}"]
    .Request()
    .GetAsync();

```