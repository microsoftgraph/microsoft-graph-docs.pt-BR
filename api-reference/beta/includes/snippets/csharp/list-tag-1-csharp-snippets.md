---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 776d393abd9bdd79e37e4a0e3b0d24440b68c3bb31c93aa116846a0b81aa88a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tags = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags
    .Request()
    .GetAsync();

```