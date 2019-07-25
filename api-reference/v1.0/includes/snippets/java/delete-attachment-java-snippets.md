---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd41b14612a6a227d641dc9231b81f91f3fecc47
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882579"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().events("{id}").attachments("{id}")
    .buildRequest()
    .delete();

```