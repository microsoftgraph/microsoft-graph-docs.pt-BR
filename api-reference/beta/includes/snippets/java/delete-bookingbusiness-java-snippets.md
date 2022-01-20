---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27ae8f9864d346c44b93c9e3cd920ea5db47e8c7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130139"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("fabrikam@contoso.onmicrosoft.com")
    .buildRequest()
    .delete();

```