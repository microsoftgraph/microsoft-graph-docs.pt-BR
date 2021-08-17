---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 234fa4bb361d161070d09e335182aa0dc051fc55efbbd857c6ab27ce66608825
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103009"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage members = graphClient.groups("{id}").members()
    .buildRequest()
    .get();

```