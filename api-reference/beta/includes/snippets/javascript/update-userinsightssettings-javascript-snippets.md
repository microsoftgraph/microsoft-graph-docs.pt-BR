---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4acc812764e34769aa26d3f1ae61578db26ee53d215187c6c4c44a46dc9e4f27
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160042"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userInsightsSettings = {
  isEnabled: 'false'
};

await client.api('/users/{userId}/settings/itemInsights')
    .version('beta')
    .update(userInsightsSettings);

```