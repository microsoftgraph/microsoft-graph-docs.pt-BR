---
title: Atualizar ediscoveryCase
description: Atualize as propriedades de um objeto ediscoveryCase.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: fe63000529f9fc88363efad080678d65beb03b29
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839026"
---
# <a name="update-ediscoverycase"></a>Atualizar ediscoveryCase
Namespace: microsoft.graph.security



Atualize as propriedades de [um objeto ediscoveryCase](../resources/security-ediscoverycase.md) .

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
PATCH /security/cases/ediscoveryCases/{ediscoveryCaseId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação


No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|A descrição do caso.|
|displayName|String|O nome do caso.|
|externalId|Cadeia de caracteres|O número de caso externo para referência de cliente.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 NO CONTENT`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "update_ediscoverycase"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/22aa2acd-7554-4330-9ba9-ce20014aaae4
Content-Type: application/json

{
    "displayName": "My Case 1 - Renamed",
    "description": "Updated description"
}
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```
