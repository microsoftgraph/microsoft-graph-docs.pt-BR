---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f164cbf0abba790724e05ea585a193b879127912
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channel = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2')
    .get();

```