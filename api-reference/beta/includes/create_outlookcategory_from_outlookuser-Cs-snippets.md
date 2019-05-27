---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c508364eaa7b2727b139d26a30b2bc97e732b643
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440146"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookCategory = new OutlookCategory
{
    DisplayName = "Project expenses",
    Color = CategoryColor.Preset9
};

await graphClient.Me.Outlook.MasterCategories
    .Request()
    .AddAsync(outlookCategory);

```