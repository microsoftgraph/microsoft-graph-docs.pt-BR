---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b58fc24d840cc773436f08837c4280c33f0ecc9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982953"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}")
    .buildRequest()
    .delete();

```