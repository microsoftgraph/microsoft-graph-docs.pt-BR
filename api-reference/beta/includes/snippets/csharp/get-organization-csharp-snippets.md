---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6c801d93e949b5aa883ab18719c1b4ca9aed6f8f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618746"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organization = await graphClient.Organization
    .Request()
    .GetAsync();

```