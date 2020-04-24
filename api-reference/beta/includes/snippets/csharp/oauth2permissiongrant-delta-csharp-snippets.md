---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46fc470f13844e0d452a9002ad432a2bdae3eda9
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Oauth2permissiongrants
    .Delta()
    .Request()
    .GetAsync();

```