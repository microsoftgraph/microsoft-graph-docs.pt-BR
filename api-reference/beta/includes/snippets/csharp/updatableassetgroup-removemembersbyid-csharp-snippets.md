---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5672a6da30c6de05876c3e9be0d8b577e62718a4b8da4e17754f70bca3b3554
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "String",
    "String",
    "String"
};

var memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";

await graphClient.Admin.Windows.Updates.UpdatableAssets["{windowsUpdates.updatableAsset-id}"]
    .RemoveMembersById(ids,memberEntityType)
    .Request()
    .PostAsync();

```