---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4bb08d4d28cd7259f8fa19cf763b9596da74d05
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.Education.Classes["{educationClass-id}"].Assignments
    .Request()
    .GetAsync();

```