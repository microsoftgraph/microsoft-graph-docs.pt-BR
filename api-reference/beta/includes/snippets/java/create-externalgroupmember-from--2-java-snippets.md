---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc2827237710bdf3b59c9d8edfeff73126e176fa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955995"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroupMember externalGroupMember = new ExternalGroupMember();
externalGroupMember.id = "e5477431-1038-484e-bf69-1dfedb97a110";
externalGroupMember.type = ExternalGroupMemberType.GROUP;
externalGroupMember.identitySource = IdentitySourceType.AZURE_ACTIVE_DIRECTORY;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(externalGroupMember);

```