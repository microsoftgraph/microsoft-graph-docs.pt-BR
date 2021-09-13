---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8649377c2f797579bb55466ca8b55a6bc959fbc79fb0e140633f59c393b48de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158970"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let homeRealmDiscoveryPolicy = await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .get();

```