---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec555257103504d3798c219000de75b26837c298
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let adminConsentRequestPolicy = await client.api('/policies/adminConsentRequestPolicy')
    .get();

```