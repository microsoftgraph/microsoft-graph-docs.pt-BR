---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1e7ddfce69f798c85847e387f95fa39b6f41326
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179578"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGE1M2_bs88AACHsLqWAAA="]
    .Request()
    .Expand("singleValueExtendedProperties($filter=id%20eq%20'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color')")
    .GetAsync();

```