---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 212db15d580961efd17f0644220adcb08b9a2a62
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980115"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("{id}").owners("{id}").reference()
    .buildRequest()
    .delete();

```