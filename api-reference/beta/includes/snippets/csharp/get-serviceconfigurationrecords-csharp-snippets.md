---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dba15723bd2de0d3b1414bbe02bfb7c837615dc8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceConfigurationRecords = await graphClient.Domains["contoso.com"].ServiceConfigurationRecords
    .Request()
    .GetAsync();

```