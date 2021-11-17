---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e25d9383ba5e972c24855654aeb5c74ec57543d0cf2074ed1873b394c69037d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatableAsset = await graphClient.Admin.Windows.Updates.UpdatableAssets["{windowsUpdates.updatableAsset-id}"]
    .Request()
    .GetAsync();

```