---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 991fc7fdb44c0af9bd4567da5e09e55983deb958
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var storageLocation = "storageLocation-value";

await graphClient.Users["{id}"]
    .ExportPersonalData(storageLocation)
    .Request()
    .PostAsync();

```