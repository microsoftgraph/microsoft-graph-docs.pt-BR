---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6ee3e2e4c929e4a593493b09e405da1dd4e1c1d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137508"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Identity identity = new Identity();
identity.id = "e811976d-83df-4cbd-8b9b-5215b18aa874";
identity.type = IdentityType.USER;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(identity);

```