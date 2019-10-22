---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a27f251232fe3f8cac26da65b54d78ba0caa06fa
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2019
ms.locfileid: "35890706"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .buildRequest()
    .delete();

```