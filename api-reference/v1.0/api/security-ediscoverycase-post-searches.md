---
title: Criar pesquisas
description: Crie um novo objeto ediscoverySearch.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 9ba83f967e346606d8f38075c3a373add2004203
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839215"
---
# <a name="create-searches"></a>Criar pesquisas
Namespace: microsoft.graph.security



Crie um novo [objeto ediscoverySearch](../resources/security-ediscoverysearch.md) .

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON [do objeto ediscoverySearch](../resources/security-ediscoverysearch.md) .

Você pode especificar as propriedades a seguir ao criar **um ediscoverySearch**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da pesquisa. Obrigatório|
|descrição|String|A descrição da pesquisa Opcional.|
|contentQuery|Cadeia de caracteres|A cadeia de caracteres de consulta usada para a pesquisa. A cadeia de caracteres de consulta no formato KQL (Linguagem de Consulta de Palavra-chave). Opcional|
|dataSourceScopes|microsoft.graph.security.dataSourceScopes|A opção de pesquisar em todas as caixas de correio ou sites no locatário. Os valores possíveis são: `none`, `allTenantMailboxes`, `allTenantSites`, `allCaseCustodians`, `allCaseNoncustodialDataSources`. Opcional.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um [objeto microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_ediscoverysearch_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches
Content-Type: application/json

{
    "displayName": "My search 2",
    "description": "My first search",
    "contentQuery": "(Author=\"edison\")",
    "custodianSources@odata.bind": [
        "https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/userSources/43434642-3137-3138-3432-374142313639",
        "https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/siteSources/169718e3-a8df-449d-bef4-ee09fe1ddc5d",
        "https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources('32e14fa4-3106-4bd2-a245-34bf0c718a7e')"
    ],
    "noncustodialSources@odata.bind": [
        "https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/35393639323133394345384344303043"
    ]
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoverySearch"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/searches/$entity",
    "dataSourceScopes": "none",
    "description": "My first search",
    "lastModifiedDateTime": "2022-05-23T04:38:07.5787454Z",
    "contentQuery": "(Author=\"edison\")",
    "id": "46867792-68e6-41db-9cd0-f651c2290d91",
    "displayName": "My search 2",
    "createdDateTime": "2022-05-23T04:38:07.5787454Z",
    "lastModifiedBy": null,
    "createdBy": {
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": "MOD Administrator",
            "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
        },
        "application": {
            "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "displayName": "Graph Explorer"
        }
    }
}
```

