---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eceb0320260c77ebab0fb70a114034aaedb1eb0d
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226779"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomSecurityAttributeDefinition customSecurityAttributeDefinition = new CustomSecurityAttributeDefinition();
customSecurityAttributeDefinition.attributeSet = "Engineering";
customSecurityAttributeDefinition.description = "Active projects for user";
customSecurityAttributeDefinition.isCollection = true;
customSecurityAttributeDefinition.isSearchable = true;
customSecurityAttributeDefinition.name = "Project";
customSecurityAttributeDefinition.status = "Available";
customSecurityAttributeDefinition.type = "String";
customSecurityAttributeDefinition.usePreDefinedValuesOnly = true;

graphClient.directory().customSecurityAttributeDefinitions()
    .buildRequest()
    .post(customSecurityAttributeDefinition);

```