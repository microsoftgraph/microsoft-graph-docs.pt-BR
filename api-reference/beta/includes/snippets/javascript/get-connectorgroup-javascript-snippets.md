---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea553cad1837bca1eb7b41d92d241a0625df7237
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}')
    .version('beta')
    .get();

```