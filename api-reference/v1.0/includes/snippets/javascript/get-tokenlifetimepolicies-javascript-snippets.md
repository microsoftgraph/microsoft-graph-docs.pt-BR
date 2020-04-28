---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c39f1e3a47d1d154666456f8524594354b7f129f
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43718543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenLifetimePolicies')
    .get();

```