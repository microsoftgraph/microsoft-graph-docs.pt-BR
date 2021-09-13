---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24b40e4bd797e8809ae70f9f334a4633d319beb3ac1d08d400e9b021c83bbe30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let alert = await client.api('/security/alerts/{alert_id}')
    .get();

```