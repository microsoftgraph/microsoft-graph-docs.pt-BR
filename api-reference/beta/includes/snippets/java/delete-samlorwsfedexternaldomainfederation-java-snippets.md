---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66ae7defd82d4d35b7f1f284e46b45735bb0d969
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765003"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().federationConfigurations("96db02e2-80c1-5555-bc3a-de92ffb8c5be")
    .buildRequest()
    .delete();

```