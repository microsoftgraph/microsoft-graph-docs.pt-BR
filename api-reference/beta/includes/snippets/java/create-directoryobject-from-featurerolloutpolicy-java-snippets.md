---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13d99c63a23b8b190780e2851a36e7edea812556
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954519"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "2441b489-4f12-4882-b039-8f6006bd66da";

graphClient.directory().featureRolloutPolicies("{id}").appliesTo().references()
    .buildRequest()
    .post(directoryObject);

```