---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7fd9e249e0ab6846713dd1eba99b904f551edc9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858413"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage members = graphClient.groups("{id}").members()
    .buildRequest()
    .get();

```