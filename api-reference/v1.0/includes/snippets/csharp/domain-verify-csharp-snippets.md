---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0c202100b57521b76aa8877d6e1409636413a6ca92b43ea496edaab43b2c9c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["{domain-id}"]
    .Verify()
    .Request()
    .PostAsync();

```