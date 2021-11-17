---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee404a09a1f929cac4a94490cea5f3cab4862f83f9aa45dcbdd61d5fbab314c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100384"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "5793aa3b-cca9-4794-679a240f8b58";

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .GetPasswordSingleSignOnCredentials(id)
    .Request()
    .PostAsync();

```