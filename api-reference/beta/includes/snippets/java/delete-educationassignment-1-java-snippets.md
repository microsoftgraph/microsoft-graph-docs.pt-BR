---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 329c46a16b158a3dbdb0cccde881ab733ad54255
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508163"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("c42f493f-42b4-4e7d-8148-af894cbc518b").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8")
    .buildRequest()
    .delete();

```