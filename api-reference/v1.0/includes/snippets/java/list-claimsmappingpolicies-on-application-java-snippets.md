---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcf94271494bfdb4ba078ccce680228fe16a411b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863615"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IClaimsMappingPolicyCollectionPage claimsMappingPolicies = graphClient.servicePrincipals("{id}").claimsMappingPolicies()
    .buildRequest()
    .get();

```