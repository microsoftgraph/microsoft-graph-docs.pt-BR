---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12a62295105f4b6e121e20e4036b5cf8762a09589db1dfc6bc070bfea007e675
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406855"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Users["{user-id}"].MemberOf
    .Request()
    .GetAsync();

```