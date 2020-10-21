---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d833b357aafbdb88eb518f16c68109b4774f9ad
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612137"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var thumbnails = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails
    .Request()
    .GetAsync();

```