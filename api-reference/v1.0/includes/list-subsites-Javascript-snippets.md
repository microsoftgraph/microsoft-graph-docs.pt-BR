---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec12617f91b4022c416cd7edb484c8408e55d2eb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451598"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/sites')
    .get();

```