---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9702795737d7b370ed8999458513e984e0384904
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Me.Drive
    .Request()
    .GetAsync();

```