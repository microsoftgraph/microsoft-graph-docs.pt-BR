---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9019b94941846e9ded0cafad5af907a1caa9625e
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members')
    .version('beta')
    .get();

```