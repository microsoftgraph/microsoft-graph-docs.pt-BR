---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd93fcc5fce08fae7eec9ea015e16ec98cdadcda
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983897"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().connectors("{id}")
    .buildRequest()
    .delete();

```