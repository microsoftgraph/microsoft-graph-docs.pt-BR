---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae7bca24f5aeb227de92517d6d6bc79d754a2126
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979671"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintSettings printSettings = graphClient.customRequest("/print/settings", PrintSettings.class)
    .buildRequest()
    .get();

```