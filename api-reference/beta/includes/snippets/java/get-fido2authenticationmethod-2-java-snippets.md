---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 419f5492ed2771a3889f9d334262bbb4ee1ac06d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210088"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Fido2AuthenticationMethodCollectionPage fido2Methods = graphClient.me().authentication().fido2Methods()
    .buildRequest()
    .get();

```