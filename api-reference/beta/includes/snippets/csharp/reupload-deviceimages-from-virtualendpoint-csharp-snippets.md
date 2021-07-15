---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd22c9a531563860902816d1dee164a0699f4fd8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439481"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages["{cloudPcDeviceImage-id}"]
    .Reupload()
    .Request()
    .PostAsync();

```