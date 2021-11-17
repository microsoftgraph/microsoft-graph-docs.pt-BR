---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 279c5fb657f5dabff6620905adab00fb972735b8dabade4539e928d0798e6d6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214879"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"]
    .Release()
    .Request()
    .PostAsync();

```