---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e43bd871e9074ca1947a8dc6884e8c970c64d831
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210139"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("10001").classes("11001")
    .buildRequest()
    .delete();

```