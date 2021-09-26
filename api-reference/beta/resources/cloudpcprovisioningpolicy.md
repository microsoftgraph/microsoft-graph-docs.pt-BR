---
title: Tipo de recurso cloudPcProvisioningPolicy
description: Representa uma política de provisionamento de computador na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3fd07bc2df93e57d6135a3bf7956f931db13c801
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763048"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>Tipo de recurso cloudPcProvisioningPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de provisionamento de computador na nuvem.

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
|id|String|Identificador exclusivo para a política de provisionamento do Cloud PC. Somente leitura.|
|displayName|String|O nome de exibição da política de provisionamento.|
|description|Cadeia de caracteres|A descrição da política de provisionamento.|
|onPremisesConnectionId|String|A ID do cloudPcOnPremisesConnection. Para garantir que os computadores na nuvem tenham conectividade de rede e que eles participem do domínio, escolha uma conexão com uma rede virtual validada pelo serviço de Computador na Nuvem.|
|imageId|String|A ID da imagem do sistema operacional que você deseja provisionar em PCs na Nuvem. O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}. Os valores com suporte para cada um dos parâmetros são os seguinte:<ul><li>publisher: Microsoftwindowsdesktop.</li> <li>offer: windows-ent-cpc.</li> <li>sku: 21h1-ent-cpc-m365, 21h1-ent-cpc-os, 20h2-ent-cpc-m365, 20h2-ent-cpc-os, 20h1-ent-cpc-m365, 20h1-ent-cpc-os, 19h2-ent-cpc-m365 e 19h2-ent-cpc-os.</li></ul>|
|imageDisplayName|Cadeia de caracteres|O nome de exibição da imagem do sistema operacional que você está provisionando.|
|imageType|cloudPcProvisioningPolicyImageType|O tipo de imagem do sistema operacional (personalizada ou galeria) que você deseja provisionar em PCs na Nuvem. Os valores possíveis são: `gallery`, `custom`.|

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
