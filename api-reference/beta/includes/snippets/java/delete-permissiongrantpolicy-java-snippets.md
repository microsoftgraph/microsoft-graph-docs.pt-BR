---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b495fd2a7e3d5ae7d462479631ad56366c48fab2093a4ebb8e4cc42fe7608401
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326720"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy")
    .buildRequest()
    .delete();

```