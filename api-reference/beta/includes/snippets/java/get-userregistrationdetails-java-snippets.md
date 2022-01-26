---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 240924374b42790f5783264155b3dbd8023f2448
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224720"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserRegistrationDetails userRegistrationDetails = graphClient.reports().authenticationMethods().userRegistrationDetails("{userRegistrationDetailsId}")
    .buildRequest()
    .get();

```