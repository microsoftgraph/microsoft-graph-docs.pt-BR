---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a62208345272abc728092167f2866f693d5d6da2
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttribute = {
  description: "Your new hobby"
};

let res = await client.api('/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby')
    .version('beta')
    .update(identityUserFlowAttribute);

```