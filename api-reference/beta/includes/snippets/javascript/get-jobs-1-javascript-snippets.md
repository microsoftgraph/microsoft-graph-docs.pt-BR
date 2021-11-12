---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8dcf1903d8aac241b41455c6ae6b5feaacc32d17b9c70d6e3c61fd79e3bf2db0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/print/printers/{id}/jobs')
    .version('beta')
    .get();

```