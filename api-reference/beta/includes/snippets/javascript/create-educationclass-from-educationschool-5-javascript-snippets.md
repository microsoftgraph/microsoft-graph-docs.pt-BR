---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 427333e14412a6e37568cb249e46cd2977a1e2bca09f70184d7a7f73cfa86d90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
 '@odata.id':'https://graph.microsoft.com/beta/education/classes/11006'
};

await client.api('/education/schools/10002/classes/$ref')
    .version('beta')
    .post(educationClass);

```