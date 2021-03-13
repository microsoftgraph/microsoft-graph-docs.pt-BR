---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c939cc9328006f9257da7cc381e41df224e72480
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var verificationDnsRecords = await graphClient.Domains["{domain-id}"].VerificationDnsRecords
    .Request()
    .GetAsync();

```