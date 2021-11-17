---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b33ffb7edd94155539c8e33714229f8f5e35c0f9e89416a729fe14f404a5be60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101767"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSetQuery = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"].Queries["{ediscovery.reviewSetQuery-id}"]
    .Request()
    .GetAsync();

```