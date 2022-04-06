---
title: Criar cloudPcProvisioningPolicy
description: Crie uma nova política de provisionamento do Cloud PC.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c8ceafcd70592f4f0b10e1818200021cfb7ae061
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722801"
---
# <a name="create-cloudpcprovisioningpolicy"></a>Criar cloudPcProvisioningPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CloudPC.ReadWrite.All|

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

No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [o cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição da política de provisionamento.|
|descrição|String|A descrição da política de provisionamento.|
|onPremisesConnectionId|String|A ID do cloudPcOnPremisesConnection. Para garantir que os computadores na nuvem tenham conectividade de rede e que eles participem do domínio, escolha uma conexão com uma rede virtual validada pelo serviço de Computador na Nuvem.|
|imageId|String|A ID da imagem do sistema operacional que você deseja provisionar em PCs na Nuvem. O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}. Os valores com suporte para cada um dos parâmetros são os seguinte:<ul><li>publisher: Microsoftwindowsdesktop.</li> <li>offer: windows-ent-cpc.</li> <li>sku: 21h1-ent-cpc-m365, 21h1-ent-cpc-os, 20h2-ent-cpc-m365, 20h2-ent-cpc-os, 20h1-ent-cpc-m365, 20h1-ent-cpc-os, 19h2-ent-cpc-m365 e 19h2-ent-cpc-os.</li></ul>|
|imageDisplayName|String|O nome de exibição da imagem do sistema operacional que você está provisionando.|
|imageType|cloudPcProvisioningPolicyImageType|O tipo de imagem do sistema operacional (personalizada ou galeria) que você deseja provisionar em PCs na Nuvem. Os valores possíveis são: `gallery` e `custom`.|
|windowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|Configurações Windows específicas a ser configuradas durante a criação de PCs na Nuvem para essa política de provisionamento.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcprovisioningpolicy_from_cloudpcprovisioningpolicy"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "description": "Description value",
    "displayName": "Display Name value",
    "domainJoinConfiguration": {
        "domainJoinType": "hybridAzureADJoin",
        "onPremisesConnectionId": "16ee6c71-fc10-438b-88ac-daa1ccafffff"
    },
    "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
    "imageDisplayName": "Windows-10 19h1-evd",
    "imageId": "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
    "imageType":"gallery",
    "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
    "windowsSettings": {
        "language": "en-US"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "domainJoinConfiguration": {
      "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
      "type": "hybridAzureADJoin"
  },
  "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
  "imageDisplayName": "Windows-10 19h1-evd",
  "imageId": "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
  "imageType":"gallery",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "windowsSettings": {
    "language": "en-US"
  }
}
```
