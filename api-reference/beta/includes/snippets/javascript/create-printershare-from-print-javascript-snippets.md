---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b28d293e44dcabdc0c7e6816c18b4783b8090afe
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  name: "name-value",
  printer@odata.bind: "https://graph.microsoft.com/beta/print/printers/{id}"
};

let res = await client.api('/print/shares')
    .version('beta')
    .post(printerShare);

```