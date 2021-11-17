---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5931e089d6719c489e79856c9e7777fbeed1aed43247507ed85c99fc54629460
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userSources = await client.api('/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/userSources')
    .version('beta')
    .get();

```