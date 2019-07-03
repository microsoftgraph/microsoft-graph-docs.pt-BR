---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59f4a53626df8990c049714a2864ead1a39ad91b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507999"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplate = await graphClient.GroupSettingTemplates["{id}"]
    .Request()
    .GetAsync();

```