---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 725e70c55100997bf825df7a5a017b74ac83b50e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736137"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Drive.Recent()
    .Request()
    .GetAsync();

```