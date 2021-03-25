---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 761946427dce5465a8c9fcdb66ad093e75c6cd76
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210714"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailAuthenticationMethodCollectionPage emailMethods = graphClient.me().authentication().emailMethods()
    .buildRequest()
    .get();

```