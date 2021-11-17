---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bebbeecb2fb3e3dcf36fd60172e04c5812ccfdc54f8b3db1abd7f5a2266f8d94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102310"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = graphClient.identity().apiConnectors("{id}")
    .buildRequest()
    .get();

```