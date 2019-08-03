---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2cceafa9e196b1a7018a59b9bbb10e6b956f96a
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172813"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive(" https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"));

graphClient.directory().featureRolloutPolicies("{id}").appliesTo().references()
    .buildRequest()
    .post(directoryObject);

```