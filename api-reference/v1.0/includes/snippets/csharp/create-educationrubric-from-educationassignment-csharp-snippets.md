---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe6c78c817b02542db7f1d2890e5c5083c884f6b15fc178e9f53b4bd6fcd0456
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Rubric.Reference
    .Request()
    .PutAsync("ceb3863e-6912-4ea9-ac41-3c2bb7b6672d");

```