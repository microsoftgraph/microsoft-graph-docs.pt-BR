---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 754084a9514e1f7b26bc62c084812f16a989e332
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059804"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage acceptedSenders = graphClient.groups("{id}").acceptedSenders()
    .buildRequest()
    .get();

```