---
title: Atualizar legalHold
description: Atualize as propriedades de um objeto legalHold.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6f44bc276bdc3ae5f23ce3243127a38d4e7a6063
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445782"
---
# <a name="update-legalhold"></a>Atualizar legalHold

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto legalHold.](../resources/ediscovery-legalhold.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
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
|contentQuery|String|Consulta KQL que especifica o conteúdo a ser mantido nos locais especificados. Para obter mais informações sobre KQL na Descoberta Digital, consulte Consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo [e Descoberta Digital.](/microsoft-365/compliance/keyword-queries-and-search-conditions) Para manter todo o conteúdo nos locais especificados, deixe **contentQuery em** branco. |
|descrição|String| A descrição de espera legal. |
|displayName|String| O nome de exibição da ressução legal. |
|isEnabled|Booliano|Indica se a espera está habilitada e mantendo o conteúdo ativamente. |

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_legalhold"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
Content-Type: application/json
Content-length: 295

{
  "description": "This is a description for a legalHold"
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 204 No Content
```
