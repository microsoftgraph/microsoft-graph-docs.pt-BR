---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed3748eb165161e9fedfc705f1889631879b4283
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Programs["7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"]
    .Request()
    .DeleteAsync();

```