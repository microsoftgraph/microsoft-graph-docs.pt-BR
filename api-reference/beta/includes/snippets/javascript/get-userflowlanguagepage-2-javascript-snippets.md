---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10849ad3e61eec42c6f2f2e0c3efbccd73478791
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955172"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let overridesPages = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages')
    .version('beta')
    .get();

```