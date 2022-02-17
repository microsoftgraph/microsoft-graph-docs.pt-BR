---
title: Tipo de recurso virtualEndpoint
description: O recurso virtualEndpoint representa um contêiner para a funcionalidade de gerenciamento de computador na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c2e31e7561685e8ad1ca7f9b58bbfcd600c3ce78
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878656"
---
# <a name="virtualendpoint-resource-type"></a>Tipo de recurso virtualEndpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner para APIs para gerenciar PCs na Nuvem.

Use a API do Cloud PC para provisionar e gerenciar áreas de trabalho virtuais para funcionários em uma organização ou junto com a [API do Intune](../resources/intune-graph-overview.md) para gerenciar pontos de extremidade físicos e virtuais.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter permissões efetivas](../api/virtualendpoint-geteffectivepermissions.md)|Coleção de cadeias de caracteres|Exibir as permissões efetivas do usuário autenticado no momento.|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[Coleção cloudPC](../resources/cloudpc.md)|Listar propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .|
|[Listar deviceImages](../api/virtualendpoint-list-deviceimages.md)|[Coleção cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Listar as propriedades e as relações dos [objetos cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[List galleryImages](../api/virtualendpoint-list-galleryimages.md)|[Coleção cloudPcGalleryImage](../resources/cloudpcgalleryimage.md)|Listar as propriedades e as relações dos [objetos cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) .|
|[Criar cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Crie um novo [objeto cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[Listar onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[Coleção cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Listar propriedades e relações dos objetos [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Criar cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Crie um novo [objeto cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Listar provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[Coleção cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Listar propriedades e relações dos objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Criar cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Crie um novo [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Listar userSettings](../api/virtualendpoint-list-usersettings.md)|[Coleção cloudPcUserSetting](../resources/cloudpcusersetting.md)|Obter os recursos cloudPcUserSetting da propriedade de navegação userSettings.|
|[Criar cloudPcUserSetting](../api/virtualendpoint-post-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Crie um novo objeto cloudPcUserSetting.|
|[Listar auditEvents](../api/virtualendpoint-list-auditevents.md)|[Coleção cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Listar propriedades e relações dos objetos [cloudPcAuditEvent](../resources/cloudpcauditevent.md) .|
|[Listar supportedRegions](../api/virtualendpoint-list-supportedregions.md)|[coleção cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md)|Listar propriedades e relações dos objetos [cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md) .|
|[Listar servicePlans](../api/virtualendpoint-list-serviceplans.md)|[Coleção cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Listar propriedades e relações dos objetos [cloudPcServicePlan](../resources/cloudpcserviceplan.md) .|
|[Listar instantâneos](../api/virtualendpoint-list-snapshots.md)|[Coleção cloudPcSnapshot](../resources/cloudpcsnapshot.md)|Obter uma lista de [objetos cloudPcSnapshot](../resources/cloudpcsnapshot.md) e suas propriedades.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do ponto de extremidade virtual. Somente leitura.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|auditEvents|[Coleção cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Evento de auditoria de computador na nuvem.|
|cloudPCs|[Coleção cloudPC](../resources/cloudpc.md)|Áreas de trabalho virtuais gerenciadas na nuvem.|
|deviceImages|[Coleção cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|O recurso de imagem no Cloud PC.|
|galleryImages|[Coleção cloudPcGalleryImage](../resources/cloudpcgalleryimage.md)|O recurso de imagem da galeria no Cloud PC.|
|onPremisesConnections|[Coleção cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Uma coleção definida de informações de recursos do Azure que pode ser usada para estabelecer a conectividade de rede local para PCs na Nuvem.|
|organizationSettings|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) |As configurações da organização do Cloud PC para um locatário. |
|provisioningPolicies|[Coleção cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Política de provisionamento de computadores na nuvem.|
|servicePlans|[Coleção cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Planos de serviço de computador na nuvem.|
|instantâneos|[Coleção cloudPcSnapshot](../resources/cloudpcsnapshot.md)|Instantâneos de computador na nuvem.|
|supportedRegions|[coleção cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md)|Regiões com suporte para computador na nuvem.|
|userSettings|[Coleção cloudPcUserSetting](../resources/cloudpcusersetting.md)|Configurações do usuário do computador na nuvem. |
## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
