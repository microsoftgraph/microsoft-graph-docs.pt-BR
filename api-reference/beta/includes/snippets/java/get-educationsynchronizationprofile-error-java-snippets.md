---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3875df0741d66385b308820850362a9204bed36f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860057"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationSynchronizationErrorCollectionPage errors = graphClient.education().synchronizationProfiles("{id}").errors()
    .buildRequest()
    .get();

```