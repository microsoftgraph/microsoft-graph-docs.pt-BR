---
title: Tipo de recurso virtualEndpoint
description: O recurso virtualEndpoint representa um contêiner para a funcionalidade de gerenciamento de computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 929b6e1c404dad30d6009264ed8e6eb27985c9e8
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533261"
---
# <a name="virtualendpoint-resource-type"></a>Tipo de recurso virtualEndpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner para APIs gerenciar o Cloud PC.

Use a API do Cloud PC para provisionar e gerenciar áreas de trabalho virtuais para funcionários em uma organização. Use-o em conjunto com a [API do Intune](../resources/intune-graph-overview.md) para gerenciar pontos de extremidade físicos e virtuais.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter permissões efetivas](../api/virtualendpoint-geteffectivepermissions.md)|Coleção de cadeias de caracteres|Exibir as permissões efetivas do usuário autenticado no momento.|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[Coleção cloudPC](../resources/cloudpc.md)|Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)|
|[Listar deviceImages](../api/virtualendpoint-list-deviceimages.md)|[Coleção cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Listar as propriedades e as relações dos [objetos cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Criar cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Crie um novo [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Listar onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[Coleção cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Listar propriedades e relações dos objetos [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Criar cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Crie um novo [objeto cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Listar provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[Coleção cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Listar propriedades e relações dos objetos [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Criar cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Crie um novo [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Listar userSettings](../api/virtualendpoint-list-usersettings.md)|[Coleção cloudPcUserSetting](../resources/cloudpcusersetting.md)|Obter os recursos cloudPcUserSetting da propriedade de navegação userSettings.|
|[Criar cloudPcUserSetting](../api/virtualendpoint-post-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Crie um novo objeto cloudPcUserSetting.|
|[Listar auditEvents](../api/virtualendpoint-list-auditevents.md)|[Coleção cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Listar propriedades e relações dos objetos [cloudPcAuditEvent.](../resources/cloudpcauditevent.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da ID do ponto de extremidade virtual. Somente leitura.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|cloudPCs|[Coleção cloudPC](../resources/cloudpc.md)|Áreas de trabalho virtuais gerenciadas na nuvem.|
|deviceImages|[Coleção cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|O recurso de imagem no Cloud PC.|
|onPremisesConnections|[Coleção cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Uma coleção definida de informações de recursos do Azure que pode ser usada para estabelecer a conectividade de rede local para PCs na Nuvem.|
|provisioningPolicies|[Coleção cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Política de provisionamento de computadores na nuvem.|
|userSettings|[Coleção cloudPcUserSetting](../resources/cloudpcusersetting.md)|Configurações do usuário do computador na nuvem. |
|auditEvents|[Coleção cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Evento de auditoria de computador na nuvem.|

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
