---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de2377e20d2243129458d27ba8b99c0ea29bef28
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795447"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.TaskDefinitions["{printTaskDefinition-id}"]
    .Request()
    .DeleteAsync();

```