---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4bcbf96445f2936644c0ffc063d912ed6dcbffc4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let usageRights = await client.api('/devices/{objectId}/usageRights')
    .version('beta')
    .filter('state in (\'active\', \'suspended\') and serviceIdentifier in (\'ABCD\')')
    .get();

```