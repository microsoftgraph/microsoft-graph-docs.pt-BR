---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7be2598b798bd539ade1dfb4cbc174626c11741e591b050cff125a75470a9305
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.Education.Schools["{educationSchool-id}"].AdministrativeUnit
    .Request()
    .GetAsync();

```