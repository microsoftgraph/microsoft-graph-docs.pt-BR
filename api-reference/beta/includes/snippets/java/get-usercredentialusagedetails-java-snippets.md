---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 768f3acd19983f713b1eb6bed8500df65e52ee47
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871197"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCredentialUsageDetailsCollectionPage userCredentialUsageDetails = graphClient.reports().userCredentialUsageDetails()
    .buildRequest()
    .get();

```