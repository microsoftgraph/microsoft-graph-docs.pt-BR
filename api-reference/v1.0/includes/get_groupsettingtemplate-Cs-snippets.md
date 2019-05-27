---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59f4a53626df8990c049714a2864ead1a39ad91b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplate = await graphClient.GroupSettingTemplates["{id}"]
    .Request()
    .GetAsync();

```