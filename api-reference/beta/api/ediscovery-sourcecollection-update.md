---
title: Atualizar sourceCollection
description: Atualize as propriedades de um objeto sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 254d2422c344580e1a02dbbce0d76330d6df3ef8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445741"
---
# <a name="update-sourcecollection"></a>Atualizar sourceCollection

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto sourceCollection.](../resources/ediscovery-sourcecollection.md)

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
PATCH /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
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
|contentQuery|String|A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language). Para obter detalhes, consulte [Consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta De Conteúdo.](/microsoft-365/compliance/keyword-queries-and-search-conditions)  Você pode refinar pesquisas usando campos emparelhados com valores; por exemplo, `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016` .|
|descrição|String|A descrição da **sourceCollection**.|
|displayName|String|O nome de exibição do **sourceCollection**.|
|tenantSources|microsoft.graph.ediscovery.tenantSources|Quando especificado, a coleção se estenderá por um serviço para uma carga de trabalho inteira. Os valores possíveis são: `allMailboxes` e `allSites`.|

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_sourcecollection"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119
Content-Type: application/json
Content-length: 247

{
    "displayName": "Quarterly Financials search",
}
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
