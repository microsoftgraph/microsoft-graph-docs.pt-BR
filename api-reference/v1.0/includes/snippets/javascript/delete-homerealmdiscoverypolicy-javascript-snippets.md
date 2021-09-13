---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 296be00016fe264921b205425244aaa51195d97c9049d1de279fedaeb918d8c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .delete();

```