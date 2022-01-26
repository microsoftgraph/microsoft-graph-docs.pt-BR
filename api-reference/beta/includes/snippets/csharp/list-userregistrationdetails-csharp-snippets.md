---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 673f0d08f6e0f8448d0a09f1794ac7a29b680703
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userRegistrationDetails = await graphClient.Reports.AuthenticationMethods.UserRegistrationDetails
    .Request()
    .GetAsync();

```