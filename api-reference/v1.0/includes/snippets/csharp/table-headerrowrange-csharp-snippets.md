---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 589a7e179a9256c4630e990a8fd0d2e903bb77e4
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .HeaderRowRange()
    .Request()
    .GetAsync();

```