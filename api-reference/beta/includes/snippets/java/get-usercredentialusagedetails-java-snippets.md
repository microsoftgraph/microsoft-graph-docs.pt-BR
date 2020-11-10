---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 768f3acd19983f713b1eb6bed8500df65e52ee47
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971476"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCredentialUsageDetailsCollectionPage userCredentialUsageDetails = graphClient.reports().userCredentialUsageDetails()
    .buildRequest()
    .get();

```