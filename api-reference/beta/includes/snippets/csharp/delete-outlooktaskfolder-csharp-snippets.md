---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4e62784c2834b7e219d3b81754ac7653f4340615
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621000"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.TaskFolders["AAMkADIyAAAhrbPXAAA="]
    .Request()
    .DeleteAsync();

```