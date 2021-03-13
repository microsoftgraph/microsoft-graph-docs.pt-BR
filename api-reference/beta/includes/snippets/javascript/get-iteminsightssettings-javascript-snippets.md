---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 182287bc800cbc90d709a1601362eca674d2bfdb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemInsightsSettings = await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .get();

```