---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 810f7f790d217630202561c5de4f008e3152ccf7ff9e7e3b54b0a4d8285afa5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.Education.Classes["{educationClass-id}"].Members["{educationUser-id}"].Schools["{educationSchool-id}"].AdministrativeUnit
    .Request()
    .GetAsync();

```