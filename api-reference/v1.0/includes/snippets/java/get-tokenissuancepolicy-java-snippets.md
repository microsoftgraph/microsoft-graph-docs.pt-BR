---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76f800e7eaa6eb4f82cf16b9d35047eae2fbc0b431ce32346e7ca321673a8a9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157132"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicy tokenIssuancePolicy = graphClient.policies().tokenIssuancePolicies("{id}")
    .buildRequest()
    .get();

```