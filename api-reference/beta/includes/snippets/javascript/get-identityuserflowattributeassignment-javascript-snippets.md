---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66032485c7436c42de2561ab215eff725d6e8863
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "50435150"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2xUserFlows/{id}/userAttributeAssignments')
    .version('beta')
    .get();

```