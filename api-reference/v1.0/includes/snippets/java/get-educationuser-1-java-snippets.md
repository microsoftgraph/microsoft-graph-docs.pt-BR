---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92c5525eaabdc71f0cbbbaf3f564986b04ed7fd1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208599"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.education().me().user()
    .buildRequest()
    .get();

```