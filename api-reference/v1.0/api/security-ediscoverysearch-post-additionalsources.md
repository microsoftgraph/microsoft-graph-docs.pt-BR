---
title: Adicionar fontes adicionais
description: Crie uma nova fonte adicional associada a uma pesquisa de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 99a910cfd87bc58f60ea7a79e64ebae6bb42c6a2
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839246"
---
# <a name="add-additional-sources"></a>Adicionar fontes adicionais
Namespace: microsoft.graph.security


Crie uma nova [fonte adicional](../resources/security-datasource.md) associada a [uma pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto dataSource](../resources/security-datasource.md) .

Você pode especificar as propriedades a seguir ao criar uma **fonte de dados**.

>**Nota:** É **necessário email** **ou site** , mas não ambos. 

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|email|cadeia de caracteres|Endereço SMTP da caixa de correio. Para obter o endereço de email de um grupo, use [Grupos de lista ou](../api/group-list.md) [Obter grupo](../api/group-get.md). Você pode consultar pelo nome do grupo usando `$filter`; por exemplo, `https://graph.microsoft.com/v1.0/groups?$filter=displayName eq 'secret group'&$select=mail,id,displayName`.|
|site|cadeia de caracteres|URL do site; por exemplo, `https://contoso.sharepoint.com/sites/HumanResources`. |


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` objeto [microsoft.graph.security.dataSource](../resources/security-ediscoverysearch.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_datasource_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources

{
    "@odata.type": "microsoft.graph.security.siteSource",
    "site": {
        "webUrl": "https://contoso.sharepoint.com/sites/SecretSite"
    }
}
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.dataSource"
}
-->
``` http
HTTP/1.1 201 Created

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/searches('c61a5860-d634-4d14-aea7-d82b6f4eb7af')/additionalSources/$entity",
    "@odata.type": "#microsoft.graph.security.siteSource",
    "@odata.id": "https://graph.microsoft.com/v1.0/sites/46303732-3434-4630-3832-363333363441",
    "displayName": "Design - top secret",
    "createdDateTime": "2022-07-15T22:45:36.1096267Z",
    "holdStatus": "0",
    "id": "46303732-3434-4630-3832-363333363441",
    "createdBy": {
        "application": null,
        "user": {
            "id": null,
            "displayName": null
        }
    }
}
```
