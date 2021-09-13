---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a861ffe2c27995626fc2e2090204492d06239a2cdb269c473e4ef8103516ae7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permission = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .get();

```