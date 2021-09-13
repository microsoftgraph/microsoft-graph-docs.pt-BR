---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c7be48e636920a450ad8e3737aac96251683babd83bc9888a5fab7d45e145bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teamwork/workforceIntegrations/{workforceIntegrationId}')
    .delete();

```