---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8455ac6304b43e1bad20ccf1ad25be7b215441362a9b8999e5cb796db5862ba3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329489"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/attachments/{id}')
    .delete();

```