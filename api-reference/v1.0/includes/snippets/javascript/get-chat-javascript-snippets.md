---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb6a318efba47e7aec883e95cc091f4115971697370884c4be1a28370fbffd21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156670"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces')
    .get();

```