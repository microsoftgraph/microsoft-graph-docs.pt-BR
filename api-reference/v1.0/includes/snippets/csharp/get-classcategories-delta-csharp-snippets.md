---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9977c8a7b5116de772edac1c187558a838722197
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories
    .Delta()
    .Request()
    .GetAsync();

```