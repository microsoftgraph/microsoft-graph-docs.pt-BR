---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6458c9e05447c52e8663ceac3c84fb3b1aacb0c5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241268"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addMembers = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.UpdatableAsset
    {
        Id = "String (identifier)"
    }
};

var removeMembers = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.UpdatableAsset
    {
        Id = "String (identifier)"
    }
};

var addExclusions = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.UpdatableAsset
    {
        Id = "String (identifier)"
    }
};

var removeExclusions = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.UpdatableAsset
    {
        Id = "String (identifier)"
    }
};

await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"].Audience
    .UpdateAudience(addMembers,removeMembers,addExclusions,removeExclusions)
    .Request()
    .PostAsync();

```