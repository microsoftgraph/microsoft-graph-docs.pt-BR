---
title: Listar samlOrWsFedExternalDomainFederations
description: Obtenha uma lista dos objetos samlOrWsFedExternalDomainFederation e suas propriedades.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c21ac0212d1ced07e1c7bb78879e84747ac7c94d
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296561"
---
# <a name="list-samlorwsfedexternaldomainfederations"></a>Listar samlOrWsFedExternalDomainFederations
Namespace: microsoft.graph

Obtenha uma lista dos [objetos samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) e suas propriedades.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|Domain.Read.All, Domain.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Application|Domain.Read.All, Domain.ReadWrite.All|

A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador Global
* Administrador do Provedor de Identidade Externo

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método `200 OK` retornará um código de resposta e uma coleção de [objetos samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "list_samlorwsfedexternaldomainfederation"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.samlOrWsFedExternalDomainFederation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
    {
        "id": "96db02e2-80c1-5555-bc3a-de92ffb8c5be",
        "displayName": "Contoso",
        "issuerUri": "http://contoso.com/adfs/services/trust",
        "metadataExchangeUri": null,
        "signingCertificate": "MIIC6DCCAdCgAwIBAgIQQ6vYJIVKQ",
        "passiveSignInUri": "https://contoso.com/adfs/ls/",
        "preferredAuthenticationProtocol": "saml",
        "domains": [
            {
                "id": "contoso.com"
            }
        ]
    },
    {
        "id": "fa421032-5d40-5555-a428-a304b4bc18b6",
        "displayName": "Fabrikam",
        "issuerUri": "https://fabrikam.com/o/saml2?idpid=C018555d",
        "metadataExchangeUri": null,
        "signingCertificate": "MIIDdDCCAlygAwIBAgIGAXowJih/",
        "passiveSignInUri": "https://fabrikam.com/o/saml2/saml2?idpid=C018555d",
        "preferredAuthenticationProtocol": "wsFed",
        "domains": [
            {
                "id": "fabrikam.com",

            }
        ]
    }
  ]
}
```
