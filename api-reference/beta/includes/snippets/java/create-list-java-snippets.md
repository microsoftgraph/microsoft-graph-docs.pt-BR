---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 109dae876419c023534c0d9e2c137dbe885073e8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983756"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = new List();
list.displayName = "Books";
LinkedList<ColumnDefinition> columnsList = new LinkedList<ColumnDefinition>();
ColumnDefinition columns = new ColumnDefinition();
columns.name = "Author";
TextColumn text = new TextColumn();
columns.text = text;
columnsList.add(columns);
ColumnDefinition columns1 = new ColumnDefinition();
columns1.name = "PageCount";
NumberColumn number = new NumberColumn();
columns1.number = number;
columnsList.add(columns1);
ColumnDefinitionCollectionResponse columnDefinitionCollectionResponse = new ColumnDefinitionCollectionResponse();
columnDefinitionCollectionResponse.value = columnsList;
ColumnDefinitionCollectionPage columnDefinitionCollectionPage = new ColumnDefinitionCollectionPage(columnDefinitionCollectionResponse, null);
list.columns = columnDefinitionCollectionPage;
ListInfo list = new ListInfo();
list.template = "genericList";
list.list = list;

graphClient.sites("{site-id}").lists()
    .buildRequest()
    .post(list);

```