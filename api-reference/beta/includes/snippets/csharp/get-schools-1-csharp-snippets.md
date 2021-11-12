---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a59ea0f6a86612d916b77561ae92fe64147d263f15232add94bc70d85e41e60a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Classes["{educationClass-id}"].Schools
    .Request()
    .GetAsync();

```