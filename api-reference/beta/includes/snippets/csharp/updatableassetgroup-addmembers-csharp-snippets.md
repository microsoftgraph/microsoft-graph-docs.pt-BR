---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e9733c5b5dad6b2d0d18758a6d6dc20513bc984
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assets = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.AzureADDevice
    {
        Id = "String (identifier)"
    }
};

await graphClient.Admin.Windows.Updates.UpdatableAssets["{windowsUpdates.updatableAsset-id}"]
    .AddMembers(assets)
    .Request()
    .PostAsync();

```