---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b68ec07f7b8dcac374a56c8313e2aae48eda8636
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877846"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest()
    .get();

```