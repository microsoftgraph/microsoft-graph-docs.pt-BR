---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16192958d3a379c48adb2777f7f43de78fc07d6695eeb20f01413010cb737130
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214844"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceResourceCollectionPage resources = graphClient.privilegedAccess("azureResources").resources()
    .buildRequest()
    .get();

```