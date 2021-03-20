---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f576c566ac585cb8b1c4699564258370ce5ec12e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968672"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemReference sourceFile = new ItemReference();
SharepointIds sharepointIds = new SharepointIds();
sharepointIds.listId = "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0";
sharepointIds.listItemId = "2";
sourceFile.sharepointIds = sharepointIds;

String destinationFileName = "newname.txt";

graphClient.sites("{id}").contentTypes("{contentTypeId}")
    .copyToDefaultContentLocation(ContentTypeCopyToDefaultContentLocationParameterSet
        .newBuilder()
        .withSourceFile(sourceFile)
        .withDestinationFileName(destinationFileName)
        .build())
    .buildRequest()
    .post();

```