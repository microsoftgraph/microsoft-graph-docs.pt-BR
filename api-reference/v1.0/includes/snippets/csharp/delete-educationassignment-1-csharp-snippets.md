---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48500e0c000e8e0c319ea2db34b9935f92a52d31
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991422"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Request()
    .DeleteAsync();

```