---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 062c20f7772beed147a57f6945d7e5ef2d35b3cd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944321"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ocp-client-name", "\"My Friendly Client\""));
requestOptions.add(new HeaderOption("ocp-client-version", "\"1.2\""));

IBitlockerRecoveryKeyCollectionPage recoveryKeys = graphClient.informationProtection().bitlocker().recoveryKeys()
    .buildRequest( requestOptions )
    .get();

```