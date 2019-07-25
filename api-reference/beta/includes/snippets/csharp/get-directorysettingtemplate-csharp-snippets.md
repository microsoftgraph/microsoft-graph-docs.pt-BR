---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3abfd8a05d639136f02927226626e27ba760b0f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713258"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplate = await graphClient.DirectorySettingTemplates["{id}"]
    .Request()
    .GetAsync();

```