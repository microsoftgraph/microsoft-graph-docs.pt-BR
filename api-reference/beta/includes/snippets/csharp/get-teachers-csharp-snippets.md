---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9095f2d2b7439d99c9c4d7834bd5416846a7e69f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teachers = await graphClient.Education.Classes["11023"].Teachers
    .Request()
    .GetAsync();

```