---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 250440bc6f7dc1f26d47a01b34efe39380e0eb7bb3c094af747ce3ec016ae491
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102858"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceEndpointCollectionPage endpoints = graphClient.print().services("{id}").endpoints()
    .buildRequest()
    .get();

```