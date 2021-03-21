---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e534819d41e046901ecacd41ab269338193f7c2a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963684"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = graphClient.education().users("{user-id}")
    .buildRequest()
    .get();

```