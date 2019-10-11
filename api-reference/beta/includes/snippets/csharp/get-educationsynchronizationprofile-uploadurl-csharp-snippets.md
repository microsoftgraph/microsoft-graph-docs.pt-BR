---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec1acf04135b8fbcb80299f82d7e93128c16133f
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428727"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @string = await graphClient.Education.SynchronizationProfiles["{id}"]
    .UploadUrl()
    .Request()
    .GetAsync();

```