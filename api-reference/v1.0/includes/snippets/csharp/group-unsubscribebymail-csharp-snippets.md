---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf4c7c1966c20bcb62a1ebc680da9229e2d46fe017247827190645ae08584ca5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .UnsubscribeByMail()
    .Request()
    .PostAsync();

```