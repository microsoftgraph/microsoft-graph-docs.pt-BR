---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9f3f82849187928ada9d30047f6ab0259278bb2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975659"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2975E9B5-44CE-4E71-93D3-30F03B5AA992")
    .applyDecisions()
    .buildRequest()
    .post();

```