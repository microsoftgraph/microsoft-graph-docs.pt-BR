---
title: Atualizar continuousAccessEvaluationPolicy
description: Atualiza as propriedades de um objeto continuousAccessEvaluationPolicy.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cb6a3cbffdb8058051442b85aeb6617639ce5dd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023402"
---
# <a name="update-continuousaccessevaluationpolicy"></a>Atualizar continuousAccessEvaluationPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades de um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                    |
|:--------------------------------------|:---------------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Policy. Read. All, Policy. ReadWrite. ConditionalAccess e Application. Read. All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Policy. Read. All, Policy. ReadWrite. ConditionalAccess e Application. Read. All |

> [!NOTE]
> Essa API tem um [problema conhecido](/graph/known-issues#permissions) relacionado às permissões.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|grupos|Coleção de cadeias de caracteres|A coleção de identificadores de grupo no escopo para avaliação. Todos os grupos estão no escopo quando a coleção está vazia.|
|isEnabled|Boolean| `true` para indicar se a avaliação de acesso contínuo deve ser executada; caso contrário `false` . |
|usuários|Coleção de cadeias de caracteres|A coleção de identificadores de usuário no escopo para avaliação. Todos os usuários estão no escopo quando a coleção está vazia.|


## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_continuousaccessevaluationpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "users": [ "88139f01-1f8d-4c06-ad74-a2544cee9aee" ],
  "groups": [ "9972fb3f-7a40-49f5-85f6-129d9dfbd47a", "ea178055-4713-4d9a-a06c-ff17466b7e77"]
}
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```