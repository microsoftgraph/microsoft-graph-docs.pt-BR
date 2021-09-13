---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d404280a2bd03de7e0c85f704c81bea1b8bbe089
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147627"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemReference sourceFile = new ItemReference();
SharepointIds sharepointIds = new SharepointIds();
sharepointIds.listId = "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0";
sharepointIds.listItemId = "2";
sourceFile.sharepointIds = sharepointIds;

String destinationFileName = "newname.txt";

graphClient.sites("{siteId}").contentTypes("{contentTypeId}")
    .copyToDefaultContentLocation(ContentTypeCopyToDefaultContentLocationParameterSet
        .newBuilder()
        .withSourceFile(sourceFile)
        .withDestinationFileName(destinationFileName)
        .build())
    .buildRequest()
    .post();

```