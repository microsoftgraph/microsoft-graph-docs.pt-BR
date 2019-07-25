---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc4beaccdae032f1bd8024adcc98d3f638684a0b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877978"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage memberOf = graphClient.contacts("{id}").memberOf()
    .buildRequest()
    .get();

```