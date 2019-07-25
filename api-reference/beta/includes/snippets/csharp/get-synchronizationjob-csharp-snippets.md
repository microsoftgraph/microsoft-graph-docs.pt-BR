---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 382b5f7b10817364e410e9fa19e13e9ea2df588d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725027"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationJob = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Request()
    .GetAsync();

```