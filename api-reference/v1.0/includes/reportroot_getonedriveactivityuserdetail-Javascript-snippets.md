---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df718fa6c84c06430d9e120ba3ec0909bbad67d7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveActivityUserDetail(period='D7')')
    .get();

```