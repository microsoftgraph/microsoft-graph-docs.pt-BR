---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35b023b4367749843c783e330dabc2e745c4a221bc2407c21c3b90a353299f0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328031"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===").extensions("Com.Contoso.Referral")
    .buildRequest()
    .delete();

```