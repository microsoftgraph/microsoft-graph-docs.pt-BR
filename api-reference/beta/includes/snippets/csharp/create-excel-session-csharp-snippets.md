---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5869360510a6f6406ae73217eb789773642fd8e8
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var persistChanges = true;

await graphClient.Me.Drive.Items["{id}"].Workbook
    .CreateSession(persistChanges,null)
    .Request()
    .PostAsync();

```