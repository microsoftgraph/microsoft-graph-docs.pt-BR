---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7aa51faa6e16d6525b13e4d8428f78778444bd9c4fbf13da6558443c55c79d93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = graphClient.identityGovernance().termsOfUse().agreements("093b947f-8363-4979-a47d-4c52b33ee1be")
    .buildRequest()
    .expand("files")
    .get();

```