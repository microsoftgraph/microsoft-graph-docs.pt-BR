---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56aae24ff87a15d197e6faac135f130f569f2858
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"]
    .Request()
    .DeleteAsync();

```