---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71c5a2f00fd028a19c63c16653f80ab77d624582
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRoot = await graphClient.Education
    .Request()
    .GetAsync();

```