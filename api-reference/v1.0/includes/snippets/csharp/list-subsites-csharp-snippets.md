---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd5605e95268e9f85c8cc1ebc08fd259c2301fca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507816"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites["{site-id}"].Sites
    .Request()
    .GetAsync();

```