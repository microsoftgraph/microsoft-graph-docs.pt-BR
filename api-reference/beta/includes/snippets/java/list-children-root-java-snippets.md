---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77b692f0932c9bd3b00cbbcd6ac0ec1691664b68
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861108"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage children = graphClient.me().drive().root().children()
    .buildRequest()
    .get();

```