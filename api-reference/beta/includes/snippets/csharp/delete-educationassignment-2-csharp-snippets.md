---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4279c89ecf6a9dd2e62053b224ded21f23d56260f1aa78950d58766c1c5e1c2a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214118"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories["{educationCategory-id}"]
    .Request()
    .DeleteAsync();

```