---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 046a6eac5f6ea4387178add9838813c1dcf1da81
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991181"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Me.Rubrics["{educationRubric-id}"]
    .Request()
    .DeleteAsync();

```