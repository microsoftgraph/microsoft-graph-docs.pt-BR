---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48580926c3daa90ce0f2d774247bcb9d1983d209
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOrganizationSettings = await graphClient.DeviceManagement.VirtualEndpoint.OrganizationSettings
    .Request()
    .GetAsync();

```