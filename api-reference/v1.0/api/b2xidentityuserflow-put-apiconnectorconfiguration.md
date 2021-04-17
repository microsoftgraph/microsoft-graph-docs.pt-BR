---
title: Atualizar apiConnectorConfiguration
description: Habilita ou desabilite um conector de API para uma etapa específica em um fluxo de usuário atualizando a propriedade apiConnectorConfiguration.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8c4b7cff6c1e6221bbece4e369c928b72eae705f
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882770"
---
# <a name="update-apiconnectorconfiguration"></a>Atualizar apiConnectorConfiguration

Namespace: microsoft.graph

Atualize a [propriedade apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) em [um b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) para habilitar ou desabilitar um conector de API em um fluxo de usuário. Cada relação da [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponde a uma etapa específica no fluxo do usuário que pode ser configurada para chamar um conector de API. Você configura um conector de API para uma etapa específica de cada vez, conforme mostrado abaixo.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|IdentityUserFlow.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
* Administrador de Fluxo de Usuário de Identidade Externa

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2xUserFlows/{b2xUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON da `id` [identidadeApiConnector](../resources/identityapiconnector.md) que você deseja usar a etapa específica. Para desabilitar um conector de API, o valor pode ser {} .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a>Exemplo 1: Habilitar o conector de API para Federação pós-IDP ao se inscrever

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"   
}
```

#### <a name="response"></a>Resposta 

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a>Exemplo 2: Habilitar o conector de API para a coleção Post Attribute ao se inscrever

#### <a name="request"></a>Solicitação 

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"   
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a>Exemplo 3: Desabilitar um conector de API para a coleção Post Attribute ao se inscrever

#### <a name="request"></a>Solicitação 

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
