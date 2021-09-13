---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9c75378972e7ed1dd2e2a23df097d9c7bc20317bbbc2f800809ce15aeccf8f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workforceIntegration = await client.api('/teamwork/workforceIntegrations/{workforceintegrationid}')
    .get();

```