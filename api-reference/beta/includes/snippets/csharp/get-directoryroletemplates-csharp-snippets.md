---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 277c00a003486e33a62f8af21ffea72f8f45fa29
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplates = await graphClient.DirectoryRoleTemplates
    .Request()
    .GetAsync();

```