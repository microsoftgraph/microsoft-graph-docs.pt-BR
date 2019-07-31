---
title: Excluir synchronizationSchema
description: Exclui o esquema personalizado e redefine o esquema para a configuração padrão. Se o esquema for excluído no contexto do modelo, ele redefinirá o esquema como o padrão associado ao modelo do `factoryTag`.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 471a583851aa8e4548d2f9c66672ce54227e5d97
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977654"
---
# <a name="delete-synchronizationschema"></a>Excluir synchronizationSchema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclui o esquema personalizado e redefine o esquema para a configuração padrão. Se o esquema for excluído no contexto do modelo, ele redefinirá o esquema como o padrão associado ao modelo do `factoryTag`.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     |Directory.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) |Sem suporte.|
|Aplicativo                            |Sem suporte.| 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Tipo    | Descrição|
|:---------------|:--------|:-----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `201 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo de uma resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
