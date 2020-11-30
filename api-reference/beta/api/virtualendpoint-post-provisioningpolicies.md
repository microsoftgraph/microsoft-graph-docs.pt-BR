---
title: Criar cloudPcProvisioningPolicy
description: Criar uma nova política de provisionamento do Cloud PC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c476ef638a2a1504e04bbb414e1d330416f80a29
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378246"
---
# <a name="create-cloudpcprovisioningpolicy"></a>Criar cloudPcProvisioningPolicy

Namespace: microsoft.graph

Criar um novo objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                |
| :------------ | :------------------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição da política de provisionamento.|
|description|String|A descrição da política de provisionamento.|
|onPremisesConnectionId|Cadeia de Caracteres|A ID do cloudPcOnPremisesConnection. Para garantir que os computadores em nuvem tenham conectividade de rede e que eles ingressem no domínio, escolha uma conexão com uma rede virtual validada pelo serviço de Cloud PC.|
|imageid|Cadeia de Caracteres|A ID da imagem do sistema operacional que você deseja provisionar em PCs em nuvem. O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}.|
|imageDisplayName|Cadeia de Caracteres|O nome de exibição para a imagem do sistema operacional que você está Provisionando.|
|ImageType|cloudPcProvisioningPolicyImageType|O tipo de imagem do sistema operacional (personalizada ou galeria) que você deseja provisionar em PCs em nuvem. Os valores possíveis são: `gallery` e `custom`.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_cloudpcprovisioningpolicy_from_cloudpcprovisioningpolicy"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
Content-Type: application/json
Content-length: 309

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "gallery"
}
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
  }
```
