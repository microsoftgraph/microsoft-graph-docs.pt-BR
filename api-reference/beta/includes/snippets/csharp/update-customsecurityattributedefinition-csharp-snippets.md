---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72f857707c572d7e70ff3752778a7db631c3f104
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225627"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customSecurityAttributeDefinition = new CustomSecurityAttributeDefinition
{
    Description = "Target completion date (YYYY/MM/DD)"
};

await graphClient.Directory.CustomSecurityAttributeDefinitions["{customSecurityAttributeDefinition-id}"]
    .Request()
    .UpdateAsync(customSecurityAttributeDefinition);

```