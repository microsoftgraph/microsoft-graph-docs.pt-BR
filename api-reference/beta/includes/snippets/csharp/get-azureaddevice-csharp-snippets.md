---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94972379917009c8a278298a26204c7f6db53d41
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241094"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatableAsset = await graphClient.Admin.Windows.Updates.UpdatableAssets["{windowsUpdates.updatableAsset-id}"]
    .Request()
    .GetAsync();

```