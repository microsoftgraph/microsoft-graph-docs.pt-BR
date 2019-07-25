---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7dd9b423f55d094375edfd0dfe50b8f60c2adc50
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .GetAsync();

```