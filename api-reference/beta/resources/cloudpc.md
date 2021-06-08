---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 232ad6a8de6634f028ec59080114110c902ce184
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787496"
---
# <a name="cloudpc-resource-type"></a>Tipo de recurso cloudPC

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma área de trabalho virtual gerenciada pela nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[Coleção cloudPC](../resources/cloudpc.md)|Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)|
|[Obter cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Leia as propriedades e as relações de um [objeto cloudPC.](../resources/cloudpc.md)|
|[Reprovision](../api/cloudpc-reprovision.md)|Nenhuma|Reprovisionar um [objeto cloudPC.](../resources/cloudpc.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para o computador de nuvem. Somente leitura.|
|displayName|String|O nome de exibição do computador na nuvem.|
|imageDisplayName|String|Nome da imagem do sistema operacional que está no computador de nuvem.|
|managedDeviceId|String|A ID do dispositivo Intune do computador na nuvem.|
|managedDeviceName|String|O nome do dispositivo Intune do computador na nuvem.|
|provisioningPolicyId|String|ID da política de provisionamento do computador na nuvem.|
|provisioningPolicyName|String|A política de provisionamento que é aplicada durante o provisionamento de PCs de nuvem.|
|onPremisesConnectionName|String|A conexão local que é aplicada durante o provisionamento de PCs de nuvem.|
|servicePlanId|String|ID do plano de serviço do computador na nuvem.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviço do computador na nuvem.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Status do computador de nuvem. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Os detalhes do status do computador na nuvem.|
|userPrincipalName|String|O nome principal do usuário (UPN) do usuário atribuído ao computador de nuvem.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do computador na nuvem. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|gracePeriodEndDateTime|DateTimeOffset|A data e a hora em que o período de carência termina e o reprovisionamento/desprovisionamento acontece. Obrigatório somente se o status for `inGracePeriod` . O timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

### <a name="cloudpcstatus-values"></a>valores cloudPcStatus

|Member|Descrição|
|:---|:---|
|notProvisioned|O Cloud PC não foi provisionado.|
|provisionamento|Cloud PC provisionamento está em andamento.|
|provisionado|O Cloud PC é provisionado e pode ser acessado por usuários finais.|
|atualização|Cloud PC resize está em andamento.|
|inGracePeriod|O Cloud PC está no período de carência de uma semana antes de ser desprovisionado.|
|desprovisionamento|O Cloud PC está desprovisionando.|
|failed|A operação em Cloud PC falhou.|

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
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)"
}
```
