---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffc7dff41d0baf03830ce84737dfe9c8643685a7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryProvisioning = await graphClient.AuditLogs.DirectoryProvisioning
    .Request()
    .GetAsync();

```