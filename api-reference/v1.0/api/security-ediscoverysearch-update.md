---
title: Atualizar ediscoverySearch
description: Atualize as propriedades de um objeto ediscoverySearch.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 789fe47603f8171051e04d8e127b97c8af4860f9
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839256"
---
# <a name="update-ediscoverysearch"></a>Atualizar ediscoverySearch
Namespace: microsoft.graph.security



Atualize as propriedades de [um objeto ediscoverySearch](../resources/security-ediscoverysearch.md) .

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
PATCH /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação



|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentQuery|Cadeia de caracteres|A cadeia de caracteres de consulta na consulta KQL (Linguagem de Consulta de Palavra-chave). Para obter detalhes, consulte [consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta Eletrônica](/microsoft-365/compliance/keyword-queries-and-search-conditions).  Você pode refinar pesquisas usando campos emparelhados com valores; por exemplo, `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016`.|
|dataSourceScopes|microsoft.graph.security.dataSourceScopes|Quando especificado, a coleção abrangerá um serviço para uma carga de trabalho inteira. Os valores possíveis são: `none`,`allTenantMailboxes`,`allTenantSites`,`allCaseCustodians`,.`allCaseNoncustodialDataSources` **Nota:** Um guardião ou a especificação de dataSourceScope é necessário ao criar uma coleção de origem.|
|descrição|String|A descrição da **pesquisa de Descoberta Eletrônica**.|
|displayName|String|O nome de exibição da **pesquisa de Descoberta Eletrônica**.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "update_ediscoverysearch"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}
Content-Type: application/json

{
    "displayName": "Teams search"
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```