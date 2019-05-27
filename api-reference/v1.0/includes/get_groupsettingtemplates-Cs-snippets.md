---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44d00c7a706c3dabc1ea8b75126bc8f3cfc1d318
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463124"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplates = await graphClient.GroupSettingTemplates
    .Request()
    .GetAsync();

```