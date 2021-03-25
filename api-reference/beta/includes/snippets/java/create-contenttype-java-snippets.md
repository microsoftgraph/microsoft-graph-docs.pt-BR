---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3abd562ae4c11e861f60e694c1629c409cbfc9ff
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202041"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentType contentType = new ContentType();
contentType.name = "docSet";
contentType.description = "custom docset";
ContentType base = new ContentType();
base.name = "Document Set";
base.id = "0x0120D520";
contentType.base = base;
contentType.group = "Document Set Content Types";

graphClient.sites("{id}").contentTypes()
    .buildRequest()
    .post(contentType);

```