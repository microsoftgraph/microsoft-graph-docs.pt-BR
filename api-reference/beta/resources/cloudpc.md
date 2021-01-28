---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1b026bccd18af0dcbc9c0a5128595399a0997474
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033915"
---
# <a name="cloudpc-resource-type"></a>Tipo de recurso cloudPC

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma área de trabalho virtual gerenciada na nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[Coleção cloudPC](../resources/cloudpc.md)|Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)|
|[Obter cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Leia as propriedades e os relacionamentos de um [objeto cloudPC.](../resources/cloudpc.md)|
|[Reprovisionamento](../api/cloudpc-reprovision.md)|Nenhum|Reprovisionar um [objeto cloudPC.](../resources/cloudpc.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do computador na nuvem. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição do computador na nuvem.|
|imageDisplayName|Cadeia de caracteres|Nome da imagem do sistema operacional que está no computador em nuvem.|
|managedDeviceId|Cadeia de caracteres|A ID do dispositivo Intune do computador na nuvem.|
|managedDeviceName|String|O nome do dispositivo Intune do computador na nuvem.|
|provisioningPolicyId|Cadeia de caracteres|A ID de política de provisionamento do computador na nuvem.|
|servicePlanId|Cadeia de caracteres|A ID do plano de serviço do computador de nuvem.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviço do computador na nuvem.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Status do computador na nuvem. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Os detalhes do status do computador na nuvem.|
|userPrincipalName|Cadeia de caracteres|O nome UPN do usuário atribuído ao computador em nuvem.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do computador na nuvem. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.|

### <a name="cloudpcstatus-values"></a>Valores de cloudPcStatus

|Member|Descrição|
|:---|:---|
|notProvisioned|O Cloud PC não foi provisionado.|
|provisionamento|O provisionamento de computadores na nuvem está em andamento.|
|provisionado|O Cloud PC é provisionado e pode ser acessado por usuários finais.|
|atualização|O relize do computador na nuvem está em andamento.|
|inGracePeriod|O Cloud PC está no período de carência de uma semana antes de ser desprovisionado.|
|desprovisioning|O Cloud PC está desprovisionamento.|
|failed|A operação no Cloud PC falhou.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPC",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPC",
  "id": "String (identifier)",
  "displayName": "String",
  "imageDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```
