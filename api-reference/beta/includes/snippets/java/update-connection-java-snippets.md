---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0f518f80851c18bbf3ce3a1bdb04f4855aae508
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982353"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnection externalConnection = new ExternalConnection();
externalConnection.name = "Contoso HR Service Tickets";
externalConnection.description = "Connection to index HR service tickets";

graphClient.connections("contosohr")
    .buildRequest()
    .patch(externalConnection);

```