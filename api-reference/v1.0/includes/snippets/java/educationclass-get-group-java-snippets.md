---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac99cf2a70e24433c53dac59c325a277ddb47287
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975249"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.education().classes("{class-id}").group()
    .buildRequest()
    .get();

```