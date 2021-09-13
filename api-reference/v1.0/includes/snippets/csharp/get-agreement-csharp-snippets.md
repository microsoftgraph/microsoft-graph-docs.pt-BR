---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af02817f422d5b4bb7d4e14535fefc603de82226b5897dfaa540b83db4f4faa7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329769"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"]
    .Request()
    .Expand("files")
    .GetAsync();

```