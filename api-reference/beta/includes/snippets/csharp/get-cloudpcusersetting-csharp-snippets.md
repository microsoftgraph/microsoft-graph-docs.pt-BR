---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6190c9071bd91b17920bf11336a7fa4be036cb792ce4467bd9fbd1555cdf97df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcUserSetting = await graphClient.DeviceManagement.VirtualEndpoint.UserSettings["{cloudPcUserSetting-id}"]
    .Request()
    .GetAsync();

```