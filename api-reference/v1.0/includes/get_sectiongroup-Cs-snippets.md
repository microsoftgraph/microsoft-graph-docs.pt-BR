---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 891d096529d43d7de87fca307bb926c791f9fdc8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466250"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = await graphClient.Me.Onenote.SectionGroups["{id}"]
    .Request()
    .GetAsync();

```