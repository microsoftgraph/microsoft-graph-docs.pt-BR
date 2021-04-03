---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c70698c4e68abaaf2ee9359ade39940f3fc9d724
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/channels')
    .version('beta')
    .get();

```