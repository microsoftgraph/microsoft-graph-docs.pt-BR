---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47536e8d508afdfdd9d0a89baca120ae1f8d14784370021942323aed71cdc1ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407094"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplate = await graphClient.GroupSettingTemplates["{groupSettingTemplate-id}"]
    .Request()
    .GetAsync();

```