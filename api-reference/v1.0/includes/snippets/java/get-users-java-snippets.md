---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a976e40d5c21a01ca01273df9eb2f6c9b8f39b2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "35882796"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCollectionPage users = graphClient.users()
    .buildRequest()
    .get();

```