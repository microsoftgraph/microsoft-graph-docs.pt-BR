---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfc914da1bf86673ae729d111f9df3e677f8fc34
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59508058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.ManagedDevices["{managedDevice-id}"]
    .ResizeCloudPc(null)
    .Request()
    .PostAsync();

```