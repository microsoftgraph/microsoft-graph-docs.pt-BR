---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 928071a1f7f296a9e44c5b6862f69822edaefcf6522d89f44265e466b5c9ab92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214009"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"]
    .Request()
    .DeleteAsync();

```