---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a00efc72e71db4633bcf43afeca5c9f5f907b41d739f24c4de6a26deaa19771
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214400"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkAGI1AAAoZCfHAAA=/')
    .header('Prefer','outlook.body-content-type="text"')
    .select('subject,body,bodyPreview,uniqueBody')
    .get();

```