---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 626af6309053b41e012797b540f2ef81440bb612639c7f41875f3bd44125ab2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102150"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String contentType = "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101";

graphClient.sites("id").lists("{list-id}").contentTypes()
    .addCopy(ContentTypeAddCopyParameterSet
        .newBuilder()
        .withContentType(contentType)
        .build())
    .buildRequest()
    .post();

```