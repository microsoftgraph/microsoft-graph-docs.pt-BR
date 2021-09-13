---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e83bdace9d404384e15bd73826a5344a9e5b9510d7393aad4e2bc1daab93bddc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/dismissReminder')
    .post();

```