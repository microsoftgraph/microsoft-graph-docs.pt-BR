---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc3e4d190cc84edc7be903228c5d9d8bb10cfb10
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Root
    .Request()
    .GetAsync();

```