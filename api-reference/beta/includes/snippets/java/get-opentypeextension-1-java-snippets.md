---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34da2c5541561b382aa5f18243044d8c47a7dfeb5a6f8da42b6cc80e2df74de1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213770"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = graphClient.me().messages("AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='").extensions("Com.Contoso.Referral")
    .buildRequest()
    .get();

```