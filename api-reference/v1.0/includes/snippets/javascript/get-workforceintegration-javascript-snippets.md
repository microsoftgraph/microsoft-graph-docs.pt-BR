---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d760c957f0dfeee81fc7a2109d13d5ed4ce259b8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workforceIntegration = await client.api('/teamwork/workforceIntegrations/{workforceintegrationid}')
    .get();

```