---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97aee0ff7ac006009ce9cc67c616f789e69a5d1c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858446"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEndpointCollectionPage endpoints = graphClient.groups("{id}").endpoints()
    .buildRequest()
    .get();

```