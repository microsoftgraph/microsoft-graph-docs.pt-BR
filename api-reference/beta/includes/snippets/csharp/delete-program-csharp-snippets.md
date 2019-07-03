---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed3748eb165161e9fedfc705f1889631879b4283
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Programs["7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"]
    .Request()
    .DeleteAsync();

```