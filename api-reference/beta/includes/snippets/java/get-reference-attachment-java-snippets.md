---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 678b1eb6c4bf4deca2c00594973c469dcfc2e0c92dfdc7dd2d574b1a74c28483
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100198"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().events("AAMkAGE1M88AADUv0uAAAG=").attachments("AAMkAGE1Mg72tgf7hJp0PICVGCc0g=")
    .buildRequest()
    .get();

```