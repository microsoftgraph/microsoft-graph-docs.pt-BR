---
title: tipo de recurso cloudPcProvisioningPolicy
description: Representa uma política de provisionamento do computador de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 32a4116d6fa26109b8df57786545a0726aa7dd4e
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378216"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>tipo de recurso cloudPcProvisioningPolicy

Namespace: microsoft.graph

Representa uma política de provisionamento do computador de nuvem.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|coleção [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Listar Propriedades e relações dos objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Obter cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Leia as propriedades e os relacionamentos de um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Criar cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Criar um novo objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Atualizar cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Atualiza as propriedades de um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Excluir cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|Nenhum|Excluir um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Atribuir cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|Nenhum |Atribuir um [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) a grupos de usuários.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da política de provisionamento do Cloud PC. Somente leitura.|
|displayName|String|O nome de exibição da política de provisionamento.|
|description|String|A descrição da política de provisionamento.|
|onPremisesConnectionId|Cadeia de Caracteres|A ID do cloudPcOnPremisesConnection. Para garantir que os computadores em nuvem tenham conectividade de rede e que eles ingressem no domínio, escolha uma conexão com uma rede virtual validada pelo serviço de Cloud PC.|
|imageid|Cadeia de Caracteres|A ID da imagem do sistema operacional que você deseja provisionar em PCs em nuvem. O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}.|
|imageDisplayName|Cadeia de Caracteres|O nome de exibição para a imagem do sistema operacional que você está Provisionando.|
|ImageType|cloudPcProvisioningPolicyImageType|O tipo de imagem do sistema operacional (personalizada ou galeria) que você deseja provisionar em PCs em nuvem. Os valores possíveis são: `gallery`, `custom`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md)|Uma coleção definida de atribuições de política de provisionamento. Retornado apenas em `$expand`. Veja um [exemplo](../api/cloudpcprovisioningpolicy-get.md) de como obter a relação de atribuições. |

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
