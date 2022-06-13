---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5839e57fad7d724dc0c3af2c46e4406a4aba33aa
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"].Members["{directoryObject-id}"]
    .Request()
    .GetAsync();

```