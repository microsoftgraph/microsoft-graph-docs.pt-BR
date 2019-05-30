---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 901f492b1c78cd27eeb055f0ab1d284042786ccc
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546550"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new Extension
{
    ExtensionName = "Com.Contoso.Referral",
    CompanyName = "Wingtip Toys",
    DealValue = 500050,
    ExpirationDate = "2015-12-03T10:00:00Z"
};

await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions
    .Request()
    .AddAsync(extension);

```