---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7504f243f1abe8abf36f50dd5e495c0928f0d14157a1ca7834959ec189a9609c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoints = await graphClient.Groups["{group-id}"].Endpoints
    .Request()
    .GetAsync();

```