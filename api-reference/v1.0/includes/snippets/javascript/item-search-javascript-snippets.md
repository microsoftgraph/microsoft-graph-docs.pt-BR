---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29a768e8cb3b6087072afc602825b3dd7ea34208cdc91dabbe2cfc2ce7400b90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let search = await client.api('/me/drive/root/search(q='Contoso Project')')
    .get();

```