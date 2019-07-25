---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb19b27a7f09b8b2a8c54b6adc13bdbeb50c8f7c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889894"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage domainNameReferences = graphClient.domains("{domain-name}").domainNameReferences()
    .buildRequest()
    .get();

```