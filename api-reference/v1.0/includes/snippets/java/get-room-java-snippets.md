---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87519f761953fb32a0f6ddb9e3fb9db6dd08a62f
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332333"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Place place = graphClient.places("3162F1E1-C4C0-604B-51D8-91DA78989EB1")
    .buildRequest()
    .get();

```