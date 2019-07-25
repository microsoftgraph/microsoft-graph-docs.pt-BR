---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a196eb7596874904b7649133866414573a95016b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856523"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").conversations("AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=")
    .buildRequest()
    .delete();

```