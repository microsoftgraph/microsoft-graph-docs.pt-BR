---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89476a819b7c1b6ac3e834966e86411876d58c7939b07b8731fcaf57113852b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTask = await graphClient.Print.TaskDefinitions["{printTaskDefinition-id}"].Tasks["{printTask-id}"]
    .Request()
    .GetAsync();

```