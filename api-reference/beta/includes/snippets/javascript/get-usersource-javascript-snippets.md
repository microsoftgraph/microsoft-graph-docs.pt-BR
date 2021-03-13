---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 362d7aacf08bddccab02c2249fd3e5cd09369314
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809622"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userSources = await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources')
    .version('beta')
    .get();

```