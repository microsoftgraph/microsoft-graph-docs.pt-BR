---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89fdf13c0347789cdf856eae7228aa2a17c0acfc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616373"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationTemplates = await graphClient.ApplicationTemplates
    .Request()
    .GetAsync();

```