---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2f7b0900a63f1296c6e3df3b5c4906a03d775072d84737fa7d0611c79e02edc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327084"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UserSources
    .Request()
    .GetAsync();

```