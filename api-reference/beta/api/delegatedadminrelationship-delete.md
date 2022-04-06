---
title: Excluir delegatedAdminRelationship
description: Exclui um objeto delegatedAdminRelationship.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ab47df3c98a26931dc9decc1dd15a36e7e3bf38f
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589570"
---
# <a name="delete-delegatedadminrelationship"></a>Excluir delegatedAdminRelationship
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Exclua um objeto delegatedAdminRelationship](../resources/delegatedadminrelationship.md). Uma relação só poderá ser excluída se estiver no status "criado". 

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| DelegatedAdminRelationship.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)| Sem suporte. |
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|If-Match|If-match: {etag}. Último valor ETag conhecido para que **o delegadoAdminRelationship** seja excluído. Recupere o valor ETag de uma operação LIST ou GET. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "delete_delegatedadminrelationship"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836
If-Match: W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="
```


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

