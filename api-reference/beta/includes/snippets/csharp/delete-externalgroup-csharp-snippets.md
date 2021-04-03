---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56aae24ff87a15d197e6faac135f130f569f2858
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573043"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"]
    .Request()
    .DeleteAsync();

```