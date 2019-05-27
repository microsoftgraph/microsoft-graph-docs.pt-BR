---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dba15723bd2de0d3b1414bbe02bfb7c837615dc8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446208"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceConfigurationRecords = await graphClient.Domains["contoso.com"].ServiceConfigurationRecords
    .Request()
    .GetAsync();

```