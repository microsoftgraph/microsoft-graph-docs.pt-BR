---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74183953faffdf86300b738ee61a75cd5966c4bcfdb3296f853c69fa850fde97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["{directoryObject-id}"]
    .Request()
    .GetAsync();

```