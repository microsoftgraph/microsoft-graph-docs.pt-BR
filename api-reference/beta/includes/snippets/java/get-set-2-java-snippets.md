---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52130dc1400d549003f377313aaf270190f10312
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208938"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = graphClient.termStore().sets("{setId}")
    .buildRequest()
    .get();

```