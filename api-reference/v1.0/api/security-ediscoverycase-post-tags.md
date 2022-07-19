---
title: Criar marcas
description: Crie um novo objeto ediscoveryReviewTag.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a2892cc0aa60fc727899a95e6e33afd3929b64c0
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839251"
---
# <a name="create-tags"></a>Criar marcas
Namespace: microsoft.graph.security

Crie um novo [objeto ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/tags
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON [do objeto ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .

Você pode especificar as propriedades a seguir ao criar **um ediscoveryReviewTag**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição da marca. Obrigatório.|
|description|String|Descrição da marca. Opcional.|
|childSelectability|microsoft.graph.security.childSelectability|Esse valor controla se a experiência do usuário apresenta as marcas como caixas de seleção ou um grupo de botões de opção. Os valores possíveis são: `One`, `Many`. Obrigatório.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-tag"></a>Exemplo 1: Criar uma marca
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryreviewtag_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags

{
    "displayName": "My tag API",
    "description": "Use Graph API to create tags",
    "childSelectability": "Many"
}
```


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryReviewTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/tags/$entity",
    "displayName": "My tag API",
    "description": "Use Graph API to create tags",
    "lastModifiedDateTime": "2022-05-23T19:58:26.1573076Z",
    "childSelectability": "Many",
    "id": "7c6cc351-fb90-431f-8562-1b607a3144a4",
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

### <a name="example-2-create-a-tag-with-a-parent"></a>Exemplo 2: Criar uma marca com um pai
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryreviewtag_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags

{
    "displayName": "My tag API",
    "description": "Use Graph API to create tags",
    "childSelectability": "Many",
    "parent@odata.bind":""
}
```


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryReviewTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/tags/$entity",
    "displayName": "My tag API",
    "description": "Use Graph API to create tags",
    "lastModifiedDateTime": "2022-05-23T19:58:26.1573076Z",
    "childSelectability": "Many",
    "id": "7c6cc351-fb90-431f-8562-1b607a3144a4",
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