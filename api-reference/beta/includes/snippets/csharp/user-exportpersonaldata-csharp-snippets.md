---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83b84e2deb3461206d1a839af85eaca610d07d83
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797547"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var storageLocation = "storageLocation-value";

await graphClient.Users["{user-id}"]
    .ExportPersonalData(storageLocation)
    .Request()
    .PostAsync();

```