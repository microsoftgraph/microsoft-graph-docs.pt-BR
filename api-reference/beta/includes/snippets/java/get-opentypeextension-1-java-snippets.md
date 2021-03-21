---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08058c2674333613525f61cc9e26f37e30a69ec8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972958"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = graphClient.me().messages("AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='").extensions("Com.Contoso.Referral")
    .buildRequest()
    .get();

```