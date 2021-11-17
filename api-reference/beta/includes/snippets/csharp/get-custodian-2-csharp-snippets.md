---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 411223ec98267ea31b7784044f821bf4eaf3a2d6cee38279eea1dee6f1e376d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodian = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"]
    .Request()
    .GetAsync();

```