---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d18982b972a3c0446bd14deb9960d131331c2482
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736629"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = graphClient.me().drive().items("{id}").workbook().comments("{id}").replies("{id}")
    .buildRequest()
    .get();

```