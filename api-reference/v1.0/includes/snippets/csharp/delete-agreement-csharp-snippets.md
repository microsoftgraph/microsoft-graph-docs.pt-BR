---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1abef41db1d11f5cf296d812d02097b9d434bec9f28326043efca10f9741f18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"]
    .Request()
    .DeleteAsync();

```