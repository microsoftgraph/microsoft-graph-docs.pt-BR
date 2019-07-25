---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77ee4b7f593abf745654a2c7605e135c4e260fc2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .SubscribeByMail()
    .Request()
    .PostAsync();

```