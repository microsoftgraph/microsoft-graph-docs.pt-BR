---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4dc80e6ae11e9bf9939aee180cc6a3895016585a
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profileCardProperty = {
  annotations: [
    {
      localizations: [
        {
          languageTag: "no-NB",
          displayName: "Kostnads Senter"
        }
      ]
    }
  ]
};

let res = await client.api('/organization/{organizationId}/settings/profileCardProperties/CustomAttribute1')
    .version('beta')
    .update(profileCardProperty);

```