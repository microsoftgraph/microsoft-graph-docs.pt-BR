---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6e9da8ddbcb0855d9be6311903739693e4ddad3
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attributeSet = new AttributeSet
{
    Description = "Attributes for engineering team",
    MaxAttributesPerSet = 20
};

await graphClient.Directory.AttributeSets["{attributeSet-id}"]
    .Request()
    .UpdateAsync(attributeSet);

```