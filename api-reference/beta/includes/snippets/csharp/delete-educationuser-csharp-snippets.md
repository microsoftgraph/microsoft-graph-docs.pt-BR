---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dde4b89f6986fb698d8b14a79ba9a2eef6fc0cc0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Users["13019"]
    .Request()
    .DeleteAsync();

```