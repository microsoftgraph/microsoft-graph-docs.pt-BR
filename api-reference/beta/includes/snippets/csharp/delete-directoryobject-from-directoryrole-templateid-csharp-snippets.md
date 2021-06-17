---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2e5257a203674149fd290b54ae809d387777c60
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryRoles["{directoryRole-id}"].Members["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```