---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba7093fe0a27585ae3a400c6be79c7bf9432bada
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870390"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISecureScoreControlProfileCollectionPage secureScoreControlProfiles = graphClient.security().secureScoreControlProfiles()
    .buildRequest()
    .get();

```