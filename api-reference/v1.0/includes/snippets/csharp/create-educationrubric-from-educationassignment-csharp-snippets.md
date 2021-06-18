---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f162bbe43c52c88dfe5ad444254d9f44c00d8b5d
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992482"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Rubric.Reference
    .Request()
    .PutAsync("ceb3863e-6912-4ea9-ac41-3c2bb7b6672d");

```