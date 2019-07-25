---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7940ce68675042371ad6f39fc5df977540b80b26
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var String = await graphClient.Education.SynchronizationProfiles["{id}"]
    .UploadUrl()
    .Request()
    .GetAsync();

```