---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5739e4399892e39cba2b2e672106281a13fe7a06
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209531"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("10001").users("13006")
    .buildRequest()
    .delete();

```