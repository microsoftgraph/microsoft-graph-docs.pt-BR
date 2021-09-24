---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c32e39d8219a8ed8fd3a39c9c611888dc3128c53
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59508676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.ManagedDevices["{managedDevice-id}"]
    .ReprovisionCloudPc()
    .Request()
    .PostAsync();

```