---
title: Definir /me como singleton
description: Estas são as coisas que eu tinha para adicionar nos documentos para se certificar de que o Scanner de redução
localization_priority: Normal
ms.openlocfilehash: da71bfcb25efbebdf4e6a111f23d8d16e3aca342
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842893"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="3ef7b-103">Auxiliares (exemplos que não estão incluídos nos documentos)</span><span class="sxs-lookup"><span data-stu-id="3ef7b-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="3ef7b-104">Estas são as coisas que tive que adicionar aos documentos para garantir que a ferramenta Markdown-Scanner conseguiria lidar adequadamente com os documentos do Graph.</span><span class="sxs-lookup"><span data-stu-id="3ef7b-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="3ef7b-105">Definir /me como singleton</span><span class="sxs-lookup"><span data-stu-id="3ef7b-105">Define the /me as singleton</span></span>

<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="3ef7b-106">Defina as unidades como um conjunto de entidades consultável</span><span class="sxs-lookup"><span data-stu-id="3ef7b-106">Define drives as an queryable entityset</span></span>
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="3ef7b-107">Defina os usuários como um conjunto de entidades consultável</span><span class="sxs-lookup"><span data-stu-id="3ef7b-107">define users as an queryable entityset</span></span>

<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
