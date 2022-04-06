---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 879f7a294afd41d37d844200b326ebc116234644
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreementFile = await client.api('/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd/file')
    .version('beta')
    .get();

```