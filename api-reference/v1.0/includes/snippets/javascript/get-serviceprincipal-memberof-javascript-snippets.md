---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08b34956eb900cea7721651f1a047534c5f7c0a6d9bd13aab24d7b4bd1f89de8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216460"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/servicePrincipals/{id}/memberOf')
    .get();

```