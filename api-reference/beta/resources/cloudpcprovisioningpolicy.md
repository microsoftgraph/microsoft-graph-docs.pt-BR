---
title: Tipo de recurso cloudPcProvisioningPolicy
description: Representa uma política de provisionamento de computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b1f5a447c373e64b747fc77ec93c54d8adc09c60
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082073"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>Tipo de recurso cloudPcProvisioningPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de provisionamento de computador na nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[Coleção cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Listar propriedades e relações dos objetos [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Obter cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Leia as propriedades e as relações de um [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Criar cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Crie um novo [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Atualizar cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Atualize as propriedades de [um objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Excluir cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|Nenhum|[Exclua um objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Atribuir cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|Nenhum |Atribua [um cloudPcProvisioningPolicy a](../resources/cloudpcprovisioningpolicy.md) grupos de usuários.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a política de provisionamento de computador na nuvem. Somente leitura.|
|displayName|String|O nome de exibição da política de provisionamento.|
|description|String|A descrição da política de provisionamento.|
|onPremisesConnectionId|String|A ID do cloudPcOnPremisesConnection. Para garantir que os computadores de nuvem tenham conectividade de rede e que eles participem do domínio, escolha uma conexão com uma rede virtual validada pelo serviço de computador na nuvem.|
|imageId|String|A ID da imagem do sistema operacional que você deseja provisionar em PCs de nuvem. O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}.|
|imageDisplayName|String|O nome de exibição da imagem do sistema operacional que você está provisionando.|
|imageType|cloudPcProvisioningPolicyImageType|O tipo de imagem do sistema operacional (personalizado ou galeria) que você deseja provisionar em PCs de nuvem. Os valores possíveis são: `gallery`, `custom`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[coleção cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md)|Uma coleção definida de atribuições de política de provisionamento. Representa o conjunto de Microsoft 365 grupos e grupos de segurança no Azure AD que têm a política de provisionamento atribuída. Retornado apenas em `$expand`. Consulte um [exemplo](../api/cloudpcprovisioningpolicy-get.md) de como obter a relação de atribuições. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "onPremisesConnectionId": "String",
  "imageId": "String",
  "imageDisplayName": "String",
  "imageType": "String"
}
```
