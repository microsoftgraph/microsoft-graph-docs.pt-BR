---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80e62c6488bd25e702385992391c14627da5bfc2
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688879"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.external().connections("contosohr")
    .buildRequest()
    .delete();

```