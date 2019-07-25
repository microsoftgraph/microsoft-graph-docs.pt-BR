---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fdcafc495087b78ccc156b4fe25fdcca7b97636d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706461"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Sites["{siteId}"].Drive
    .Request()
    .GetAsync();

```