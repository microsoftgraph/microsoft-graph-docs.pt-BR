---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 910007495972723f1fdfd25961df752b8f12305c3b41b9832543b7e7f2ee0357
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329504"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicyCollectionWithReferencesPage tokenLifetimePolicies = graphClient.applications("{id}").tokenLifetimePolicies()
    .buildRequest()
    .get();

```