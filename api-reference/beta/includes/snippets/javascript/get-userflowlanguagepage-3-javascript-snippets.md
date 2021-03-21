---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34176a5f327abdc8db56daf1a4a4973b721bcb50
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages/idpselections/$value')
    .version('beta')
    .get();

```