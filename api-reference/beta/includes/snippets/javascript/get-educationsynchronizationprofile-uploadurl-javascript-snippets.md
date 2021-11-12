---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b6fd6eaac20dc85ef8bbc429c49d08bed46c47bd06656f8f31d32f1a1c6b166
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/education/synchronizationProfiles/{id}/uploadUrl')
    .version('beta')
    .get();

```