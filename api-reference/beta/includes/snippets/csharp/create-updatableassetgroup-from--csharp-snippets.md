---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29805792aba425728efa87f9270a0d94b5d1e17b8dbb16362080d844c151f807
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274988"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatableAsset = new Microsoft.Graph.WindowsUpdates.UpdatableAssetGroup
{
};

await graphClient.Admin.Windows.Updates.UpdatableAssets
    .Request()
    .AddAsync(updatableAsset);

```