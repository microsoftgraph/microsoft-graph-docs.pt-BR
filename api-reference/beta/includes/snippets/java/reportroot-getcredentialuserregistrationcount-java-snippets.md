---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d855665c6b0a1ee8eb090da59d6c8f57ccd60e34
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874097"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICredentialUserRegistrationCountCollectionPage getCredentialUserRegistrationCount = graphClient.reports()
    .getCredentialUserRegistrationCount()
    .buildRequest()
    .get();

```