---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d59241e0e2bf236a52b1f71bcfac306277e6503d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862683"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage transitiveMemberOf = graphClient.devices("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```