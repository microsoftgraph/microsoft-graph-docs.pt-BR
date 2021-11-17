---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afc66fdb29ab3bc6372ca6932ba816fea715e4b00dfbe7d4992a122710d30202
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157376"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserAccountInformationCollectionPage account = graphClient.me().profile().account()
    .buildRequest()
    .get();

```