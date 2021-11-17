---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0bd07a193224cab4cb2194716363f96327a13d1a8e01b80737ae0d38def8d62b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158883"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "2441b489-4f12-4882-b039-8f6006bd66da";

graphClient.policies().featureRolloutPolicies("{id}").appliesTo().references()
    .buildRequest()
    .post(directoryObject);

```