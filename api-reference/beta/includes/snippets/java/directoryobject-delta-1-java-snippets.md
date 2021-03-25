---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e375bfc5dbfae68a99b04d9c759cddb612118c2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208502"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

DirectoryObject directoryObject = graphClient.directoryObjects("delta")
    .buildRequest( requestOptions )
    .get();

```