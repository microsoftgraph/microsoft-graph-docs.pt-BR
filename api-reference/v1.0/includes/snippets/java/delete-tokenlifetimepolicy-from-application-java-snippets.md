---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34984666b0109ef86666cb1b27cb1d85319a28a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982246"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("{id}").tokenLifetimePolicies("{id}").reference()
    .buildRequest()
    .delete();

```