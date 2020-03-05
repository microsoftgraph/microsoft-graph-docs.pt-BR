---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 632a43b60771a3c3941a1a7c06161e6e756a88b5
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475948"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/homeRealmDiscoveryPolicies')
    .version('beta')
    .get();

```