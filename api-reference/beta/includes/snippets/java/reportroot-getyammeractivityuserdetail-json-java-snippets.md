---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5e925b9a3901745982bc12674860ab27aec7b05
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358579"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerActivityUserDetailCollectionPage getYammerActivityUserDetail = graphClient.reports()
    .getYammerActivityUserDetail("D7")
    .buildRequest()
    .get();

```