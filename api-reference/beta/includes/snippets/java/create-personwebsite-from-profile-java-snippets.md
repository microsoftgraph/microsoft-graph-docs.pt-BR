---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01465b43d2369ea0d7e81773ba1e3a90a5193f7c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980466"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonWebsite personWebsite = new PersonWebsite();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("football");
personWebsite.categories = categoriesList;
personWebsite.displayName = "Lyn Damer";
personWebsite.webUrl = "www.lyndamer.no";

graphClient.me().profile().websites()
    .buildRequest()
    .post(personWebsite);

```