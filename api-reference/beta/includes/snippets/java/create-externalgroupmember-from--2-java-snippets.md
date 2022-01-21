---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 188ab2cb9ce1326af9c00eca74ee5dce29fbe6c2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137509"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Identity identity = new Identity();
identity.id = "e5477431-1038-484e-bf69-1dfedb97a110";
identity.type = IdentityType.EXTERNAL_GROUP;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(identity);

```