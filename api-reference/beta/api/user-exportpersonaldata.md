---
title: 'usuário: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar dados de um usuário organizacionais.
ms.openlocfilehash: 27a299a4cfa6ccc3016a1f706b452840aa5dc396
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329119"
---
# <a name="user-exportpersonaldata"></a>usuário: exportPersonalData

Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar dados de um usuário organizacionais.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  User.Export.All e User.Read.All  |
|Delegado (conta pessoal da Microsoft) |  Não aplicável  |
|Application | User.Export.All e User.Read.All |

>Observação: Export só pode ser executada por um administrador da empresa ao usar a permissão delegada.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | Portador {token}|

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Type   |Descrição|
|:---------------|:--------|:----------|
|storageLocation|String|Esta é uma URL de assinatura (SAS) de acesso compartilhado para uma conta de armazenamento do Azure, para onde os dados devem ser exportados.|

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```

##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
