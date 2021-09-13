---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de87148e859fece91f97130d0d4c431df90a51858b46e9f4d20bb123858f31bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156658"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domain = await graphClient.Domains["{domain-id}"]
    .Request()
    .GetAsync();

```