---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3abfd8a05d639136f02927226626e27ba760b0f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471898"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplate = await graphClient.DirectorySettingTemplates["{id}"]
    .Request()
    .GetAsync();

```