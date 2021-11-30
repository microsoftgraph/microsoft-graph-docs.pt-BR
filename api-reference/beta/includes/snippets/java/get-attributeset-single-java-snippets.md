---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 988fab6197cadf6fb9d1e9e0ad62d91677ef5304
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223612"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttributeSet attributeSet = graphClient.directory().attributeSets("Engineering")
    .buildRequest()
    .get();

```