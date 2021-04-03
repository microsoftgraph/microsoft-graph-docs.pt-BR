---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c13bc61117032ccb54406600eb227e96876115e6
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members["{externalConnectors.externalGroupMember-id}"]
    .Request()
    .DeleteAsync();

```