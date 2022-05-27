---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 289f5e130f0d41f31c25c896aac8741bcfb2b510
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719131"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.Sites["{site-id}"].Operations
    .Request()
    .GetAsync();

```