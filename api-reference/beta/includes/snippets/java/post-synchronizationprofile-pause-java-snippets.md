---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1435c5f05ed06c3706f284a1d663e9777bd87f7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983010"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .pause()
    .buildRequest()
    .post();

```