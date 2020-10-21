---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b60eb9de0e26ffa436a8ac1183ce310b65c4dd21
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614206"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var verificationDnsRecords = await graphClient.Domains["{domain-name}"].VerificationDnsRecords
    .Request()
    .GetAsync();

```