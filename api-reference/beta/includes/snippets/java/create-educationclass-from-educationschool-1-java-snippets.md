---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88f3f94dc827958369f762d60f549c7d1858a635
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208213"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11003").members("14008")
    .buildRequest()
    .delete();

```