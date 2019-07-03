---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cea3d85ae902585f5a306c045e7685345a7c48fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499386"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions["Com.Contoso.Referral"]
    .Request()
    .DeleteAsync();

```