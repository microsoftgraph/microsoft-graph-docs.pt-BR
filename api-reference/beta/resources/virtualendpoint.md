---
title: tipo de recurso virtualEndpoint
description: O recurso virtualEndpoint representa um contêiner para a funcionalidade de gerenciamento de computador de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7e29e59658914e0f07af7635979e1b8938b99491
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563944"
---
# <a name="virtualendpoint-resource-type"></a>tipo de recurso virtualEndpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso virtualEndpoint representa um contêiner para APIs para gerenciar o computador de nuvem.

Use a API do Cloud PC para provisionar e gerenciar áreas de trabalho virtuais para os funcionários de uma organização. Use-o em conjunto com a [API do Intune](../resources/intune-graph-overview.md) para gerenciar pontos de extremidade físicos e virtuais.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter permissões efetivas](../api/virtualendpoint-geteffectivepermissions.md)|Conjunto de cadeias de caracteres|Exibir as permissões efetivas do usuário autenticado no momento.|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|coleção [cloudPC](../resources/cloudpc.md)|Listar Propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .|
|[Listar deviceImages](../api/virtualendpoint-list-deviceimages.md)|coleção [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Listar as propriedades e as relações dos objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[Criar cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Criar um novo objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[Listar onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|coleção [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Listar Propriedades e relações dos objetos [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Criar cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Criar um novo objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Listar provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|coleção [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Listar Propriedades e relações dos objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Criar cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Criar um novo objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da ID de ponto de extremidade virtual. somente leitura.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|cloudPCs|coleção [cloudPC](../resources/cloudpc.md)|Áreas de trabalho virtuais gerenciadas pela nuvem.|
|deviceImages|coleção [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|O recurso de imagem no PC de nuvem.|
|onPremisesConnections|coleção [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Uma coleção definida de informações de recursos do Azure que podem ser usadas para estabelecer conectividade de rede local para PCs em nuvem.|
|provisioningPolicies|coleção [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|política de provisionamento do Cloud PC.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
