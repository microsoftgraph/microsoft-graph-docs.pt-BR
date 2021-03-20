---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 303cc037ed77c8d3506005e2336d67932f34dbee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978740"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationalActivityCollectionPage educationalActivities = graphClient.me().profile().educationalActivities()
    .buildRequest()
    .get();

```