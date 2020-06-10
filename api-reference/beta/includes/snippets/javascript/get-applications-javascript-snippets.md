---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 312567b089b206397fd9699d3dac4115f9699eda
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications')
    .version('beta')
    .get();

```