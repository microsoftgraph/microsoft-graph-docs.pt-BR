---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 737208320865859cb794d80bf75d7f9a5f1884bb
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932390"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}").installedApps("{id}")
    .upgrade()
    .buildRequest()
    .post();

```