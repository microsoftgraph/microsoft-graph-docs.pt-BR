---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2044a060b8b4cea9c6a2c4d5132a3c999646b83
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869965"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage owners = graphClient.servicePrincipals("{id}").owners()
    .buildRequest()
    .get();

```