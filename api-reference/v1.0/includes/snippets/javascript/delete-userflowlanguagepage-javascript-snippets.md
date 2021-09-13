---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecab5d7c8e1730345affafaac4f3f61e74c2f95578cd46a615452d7203bc4c01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value')
    .version('beta')
    .delete();

```