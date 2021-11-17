---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2aec65232f57a1677fc8d46fa01169960d70ab9fe5f99b1bb27f16059fe8f88b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099697"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicies = await graphClient.Applications["{application-id}"].TokenLifetimePolicies
    .Request()
    .GetAsync();

```