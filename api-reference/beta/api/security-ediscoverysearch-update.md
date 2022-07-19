---
title: Atualizar ediscoverySearch
description: Atualize as propriedades de um objeto ediscoverySearch.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3384d11a048860df5cbae9bc003203ebd73f3c67
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838483"
---
# <a name="update-ediscoverysearch"></a>Atualizar ediscoverySearch
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentQuery|Cadeia de caracteres|A cadeia de caracteres de consulta na consulta KQL (Linguagem de Consulta de Palavra-chave). Para obter detalhes, consulte [consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta Eletrônica](/microsoft-365/compliance/keyword-queries-and-search-conditions).  Você pode refinar pesquisas usando campos emparelhados com valores; por exemplo, `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016`.|
|dataSourceScopes|microsoft.graph.security.dataSourceScopes|Quando especificado, a coleção abrangerá um serviço para uma carga de trabalho inteira. Os valores possíveis são: `none`,`allTenantMailboxes`,`allTenantSites`,`allCaseCustodians`,.`allCaseNoncustodialDataSources` **Nota:** Um guardião ou a especificação de dataSourceScope é necessário ao criar uma coleção de origem.|
|descrição|String|A descrição da **pesquisa de Descoberta Eletrônica**.|
|displayName|String|O nome de exibição da **pesquisa de Descoberta Eletrônica**.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `204 No Content` um código de resposta e um objeto [microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ediscoverysearch"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}
Content-Type: application/json

{
    "displayName": "Teams search"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ediscoverysearch-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ediscoverysearch-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-ediscoverysearch-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-ediscoverysearch-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-ediscoverysearch-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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
