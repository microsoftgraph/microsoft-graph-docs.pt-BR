---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7684d55d9b0a589c6f522017bdfd6dbd6a2a2aa43f5386e23b77092112bae571
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160305"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Buckets
    .Request()
    .GetAsync();

```