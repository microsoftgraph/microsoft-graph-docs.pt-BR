---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4946587a6d1ea73f149f5a86fb1a611696c29626f4e3823071b0bbaf11e046af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationCategory = await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories["{educationCategory-id}"]
    .Request()
    .GetAsync();

```