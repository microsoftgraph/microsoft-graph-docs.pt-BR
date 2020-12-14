---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba344de1d525d02212df2a3e3b8cf89ea902a692
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians')
    .version('beta')
    .get();

```