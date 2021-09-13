---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e237390b0afd1648f392b2edf6bc77aa98e797f22ef9b0c3b662838c50e5696c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102673"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.TokenIssuancePolicies["{tokenIssuancePolicy-id}"].AppliesTo
    .Request()
    .GetAsync();

```