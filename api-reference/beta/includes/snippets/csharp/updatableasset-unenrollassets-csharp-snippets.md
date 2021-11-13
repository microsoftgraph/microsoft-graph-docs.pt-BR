---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48ec010825deec7ba06a235d7d41273544cc4771464b53a08bd2afa60ca08ba1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updateCategory = Microsoft.Graph.WindowsUpdates.UpdateCategory.Feature;

var assets = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.AzureADDevice
    {
        Id = "String (identifier)"
    }
};

await graphClient.Admin.Windows.Updates.UpdatableAssets
    .UnenrollAssets(updateCategory,assets)
    .Request()
    .PostAsync();

```