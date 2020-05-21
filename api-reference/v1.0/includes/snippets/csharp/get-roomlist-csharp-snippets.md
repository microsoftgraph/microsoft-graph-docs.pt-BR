---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b57383ba45fdd1dbb4179ab492154a82710668b4
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332331"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = await graphClient.Places["bldg1@contoso.com"]
    .Request()
    .GetAsync();

```