---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9aca11225022e41f7a26803b263796583eff6db
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directorySettingTemplates/{id}')
    .version('beta')
    .get();

```