---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22136ee585815c96be22ff1639227cda707e994c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605643"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programControlTypes = await graphClient.ProgramControlTypes
    .Request()
    .GetAsync();

```