---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa2e10ac39be5d9414fc65e695980f39d72955ea
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871020"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "fd1c7836-4d84-4e24-b6aa-23188688cc54";

graphClient.communications().calls("{id}")
    .subscribeToTone(clientContext)
    .buildRequest()
    .post();

```