---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57da0cba02bd43776c3056d67a2450df9f6d5aee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983521"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().me().rubrics("{id}")
    .buildRequest()
    .delete();

```