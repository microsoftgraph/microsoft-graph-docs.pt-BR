---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca7c6be284d1d4057073d82570c3aa2581945328
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869929"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage memberOf = graphClient.servicePrincipals("{id}").memberOf()
    .buildRequest()
    .get();

```