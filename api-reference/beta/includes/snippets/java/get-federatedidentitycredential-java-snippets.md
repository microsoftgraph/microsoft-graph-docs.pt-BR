---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a732586168426259f27764df41211daf5f39fd33
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695194"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FederatedIdentityCredential federatedIdentityCredential = graphClient.applications("acd7c908-1c4d-4d48-93ee-ff38349a75c8").federatedIdentityCredentials("bdad0963-4a7a-43ae-b569-e67e1da3f2c0")
    .buildRequest()
    .get();

```