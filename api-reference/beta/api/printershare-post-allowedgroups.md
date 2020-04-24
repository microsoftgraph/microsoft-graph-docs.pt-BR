---
title: Criar um permitido
description: Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ce8080503f45a79dae422186ab360bc0e4071dd0
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43807061"
---
# <a name="create-allowedgroup"></a>Criar um permitido

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Users. Read. All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /print/printerShares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type  | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma referência a uma entidade de grupo usando o `@odata.id` formato, conforme mostrado no exemplo a seguir.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created`.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "create_allowedgroup_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/printerShares/{id}/allowedGroups/$ref
Content-type: application/json
Content-length: 67

{
  "@odata.id": "https://graph.microsoft.com/beta/groups/{id}"
}
```

No corpo da solicitação, forneça uma referência a uma entidade de grupo incluindo o URI do Microsoft Graph do grupo no `@odata.id` campo do corpo JSON.

### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
