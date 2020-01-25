---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1208a2ef112a943f25001c328bd00a02e87b4ea
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41496496"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Drive.Items["{id}"].Workbook.Comments["{id}"].Replies
    .Request()
    .GetAsync();

```