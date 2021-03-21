---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 042e44538f045a9329cce09bf2c84b10b196a300
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Permissions["{permission-id}"]
    .Request()
    .DeleteAsync();

```