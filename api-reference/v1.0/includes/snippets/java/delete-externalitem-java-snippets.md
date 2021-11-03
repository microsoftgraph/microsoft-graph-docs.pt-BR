---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93f36c37004c8211414af1ca5c7e854db6ce8f64
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687762"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.external().connections("contosohr").items("TSP228082938")
    .buildRequest()
    .delete();

```