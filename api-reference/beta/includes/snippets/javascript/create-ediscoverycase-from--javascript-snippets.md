---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1e72f181e507be2589c49d2600b70ff00892b3d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryCase = {
    displayName: 'CONTOSO LITIGATION-005',
    description: 'Project Bazooka',
    externalId: '324516'
};

await client.api('/security/cases/ediscoveryCases')
    .version('beta')
    .post(ediscoveryCase);

```