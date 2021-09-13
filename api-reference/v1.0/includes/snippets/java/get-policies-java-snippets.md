---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c8af57958e5fd91edd1587c29d3107f7183ed689f383376b07d10e515037d7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159504"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicyCollectionPage policies = graphClient.identity().conditionalAccess().policies()
    .buildRequest()
    .get();

```