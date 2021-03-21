---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14873d3220821460806d3314506f86b477a15d81
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980807"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnection externalConnection = new ExternalConnection();
externalConnection.id = "contosohr";
externalConnection.name = "Contoso HR";
externalConnection.description = "Connection to index Contoso HR system";

graphClient.external().connections()
    .buildRequest()
    .post(externalConnection);

```