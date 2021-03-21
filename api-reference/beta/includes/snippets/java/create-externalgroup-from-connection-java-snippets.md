---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c176ba7556a4921b40b3efae36a6fdeda36a62d1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983079"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroup externalGroup = new ExternalGroup();
externalGroup.id = "31bea3d537902000";
externalGroup.displayName = "Contoso Marketing";
externalGroup.description = "The product marketing team";

graphClient.external().connections("contosohr").groups()
    .buildRequest()
    .post(externalGroup);

```