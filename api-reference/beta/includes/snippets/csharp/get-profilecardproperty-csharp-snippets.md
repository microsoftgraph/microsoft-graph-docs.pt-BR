---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b237616a4c5299e260839355a3e65042a4a29c18
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142563"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var response = await graphClient.Organization["{organizationId}"].Settings.ProfileCardProperties["{id}"]
    .Request()
    .GetAsync();

```