---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 368cbca9e75c61021e898ca15b7e6ffd1eebccbb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880717"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ListItem listItem = new ListItem();
FieldValueSet fields = new FieldValueSet();
fields.Title = "Widget";
fields.Color = "Purple";
fields.Weight = 32;
listItem.fields = fields;

graphClient.sites("{site-id}").lists("{list-id}").items()
    .buildRequest()
    .post(listItem);

```