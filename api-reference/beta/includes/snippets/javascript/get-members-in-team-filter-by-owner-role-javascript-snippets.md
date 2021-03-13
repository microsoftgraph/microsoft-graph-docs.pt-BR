---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49ad28a6f8bd7e390bdb9039e7f746f0d5528d7c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .version('beta')
    .filter('roles/any(r:r eq \'owner\')')
    .get();

```