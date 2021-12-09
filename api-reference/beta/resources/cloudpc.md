---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e2cc53304b7fea3336e8c52874e6c2bcf772b272
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391050"
---
# <a name="cloudpc-resource-type"></a>Tipo de recurso cloudPC

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma área de trabalho virtual gerenciada pela nuvem. Esse computador cloud também está inscrito no Intune e gerenciado por meio do portal Microsoft Endpoint Manager, portanto, o Cloud PC também tem uma ID de dispositivo gerenciado correspondente do Intune.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[Coleção cloudPC](../resources/cloudpc.md)|Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)|
|[Obter cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Leia as propriedades e as relações de um [objeto cloudPC.](../resources/cloudpc.md)|
|[Reprovision](../api/cloudpc-reprovision.md)|Nenhum|Reprovisionar um [objeto cloudPC.](../resources/cloudpc.md)|
|[Fim do período de carência](../api/cloudpc-endgraceperiod.md)|Nenhum|Termine o período de carência para um [objeto cloudPC.](../resources/cloudpc.md)|
|[Reiniciar](../api/cloudpc-reboot.md)|Nenhum|Reiniciar um objeto [cloudPC](../resources/cloudpc.md) específico.|
|[Rename](../api/cloudpc-rename.md)|Nenhum|Renomeie um objeto [cloudPC](../resources/cloudpc.md) específico. Use essa API para atualizar **o displayName** para a entidade cloud pc.|
|[Solução de problemas](../api/cloudpc-troubleshoot.md)|Nenhum|Solucionar problemas de um [objeto cloudPC](../resources/cloudpc.md) específico. Use essa API para verificar o status de saúde do computador na nuvem e do host da sessão.|
|[Ação remota de reprovisionamento](../api/manageddevice-reprovisioncloudpc.md)|Nenhum|Reprovisionar um computador cloud com uma ID de dispositivo [gerenciado do](../resources/cloudpc.md) Intune.|
|[Ação remota de reprovisionamento em massa](../api/manageddevice-bulkreprovisioncloudpc.md)|Nenhum|Reprovisionar em massa um conjunto de dispositivos cloud pc com IDs de dispositivo gerenciado do Intune.|
|[Resize a ação remota](../api/manageddevice-resizecloudpc.md)|Nenhum|Atualize ou downgrade um computador cloud existente para outra configuração com novo vCPU e tamanho de armazenamento por meio da ID do dispositivo gerenciado do Intune.|
|[Obter resultados de ação remota](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Verifique os resultados da ação remota especificada pelo [computador na nuvem](../resources/cloudpcremoteactionresult.md) para um dispositivo cloud pc.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aadDeviceId|Cadeia de caracteres|A Azure Active Directory (ID de dispositivo do Azure AD) do computador cloud.|
|displayName|Cadeia de caracteres|O nome de exibição do Cloud PC.|
|gracePeriodEndDateTime|DateTimeOffset|A data e a hora em que o período de carência termina e o reprovisionamento/desprovisionamento acontece. Obrigatório somente se o status for `inGracePeriod` . O timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|id|Cadeia de caracteres|O identificador exclusivo para o Cloud PC. Apenas leitura.|
|imageDisplayName|String|Nome da imagem do sistema operacional que está no cloud pc.|
|lastLoginResult|[cloudPcLoginResult](../resources/cloudpcloginresult.md)|O último resultado de logon do Cloud PC. Por exemplo, `{ "time": "2014-01-01T00:00:00Z"}`.|
|lastModifiedDateTime|DateTimeOffset|A última data e hora modificadas do Cloud PC. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|lastRemoteActionResult|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|O último resultado de ação remota dos PCs de nuvem corporativos. As ações remotas com suporte são: `Rename` `Reboot` , , e `Reprovision` `Troubleshoot` .|
|managedDeviceId|Cadeia de caracteres|A ID do dispositivo Intune do computador cloud.|
|managedDeviceName|String|O nome do dispositivo Intune do Computador na Nuvem.|
|onPremisesConnectionName|Cadeia de caracteres|A conexão local que é aplicada durante o provisionamento de PCs na Nuvem.|
|provisioningPolicyId|Cadeia de caracteres|A ID da política de provisionamento do Cloud PC.|
|provisioningPolicyName|Cadeia de caracteres|A política de provisionamento que é aplicada durante o provisionamento de PCs de Nuvem.|
|servicePlanId|Cadeia de caracteres|A ID do plano de serviço do Cloud PC.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviço do Cloud PC.|
|servicePlanType|[cloudPcServicePlanType](../resources/cloudpcserviceplan.md#cloudpcserviceplantype-values)|O tipo de plano de serviço do Cloud PC.|
|status|[cloudPcStatus](#cloudpcstatus-values)|O status do Cloud PC. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Os detalhes do status do computador na nuvem.|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário (UPN) do usuário atribuído ao Cloud PC.|

### <a name="cloudpcstatus-values"></a>valores cloudPcStatus

|Member|Descrição|
|:---|:---|
|notProvisioned|O Cloud PC não foi provisionado.|
|provisionamento|O provisionamento do computador na nuvem está em andamento.|
|provisionado|O Cloud PC é provisionado e pode ser acessado por usuários finais.|
|inGracePeriod|O Cloud PC está no período de carência de uma semana antes de ser desprovisionado.|
|desprovisionamento|O Cloud PC está desprovisionando.|
|failed|A operação no Cloud PC falhou.|
|provisionedWithWarnings|O Cloud PC é provisionado e pode ser acessado por usuários finais, mas com alguns avisos. O usuário pode continuar a usar esse Computador na Nuvem.|
|resizing|O Cloud PC está resizing.|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

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
  "aadDeviceId": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanType": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)",
  "lastRemoteActionResult": "String",
  "lastLoginResult": "String"
}
```
