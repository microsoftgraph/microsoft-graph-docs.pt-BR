---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 994ab8cf6d7762268d9714e72036817ccbae6ae3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissions = await graphClient.Me.Drive.Items["{item-id}"].Permissions
    .Request()
    .GetAsync();

```