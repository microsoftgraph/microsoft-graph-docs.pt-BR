---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07d042e281b4762a6498ec001dbd9bb9918fc650
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712586"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = await graphClient.Education.Schools["10001"]
    .Request()
    .GetAsync();

```