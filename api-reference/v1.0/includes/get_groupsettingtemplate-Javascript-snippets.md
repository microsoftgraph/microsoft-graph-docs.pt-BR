---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69690db4ebfede451cf09b69f0582d4910d8129d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463138"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettingTemplates/{id}')
    .get();

```