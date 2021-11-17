---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8c9ef953de9f4bb8a27e2c7bdc7073fe6f19b7c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "61030357"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Conversation conversation = graphClient.groups("4d81ce71-486c-41e9-afc5-e41bf2d0722a").conversations("AAQkAGRhZmRhMWM3LTYwZTktNDZmYy1hNWU1LThhZWU4NzI2YTEyZgAQABKPPJ682apIiV1UFlj7XxY=")
    .buildRequest()
    .get();

```