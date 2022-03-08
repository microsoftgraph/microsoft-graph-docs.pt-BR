---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 9edd626ae9914941a18801791e942c1dfd69e391
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336911"
---
# <a name="cloudpc-resource-type"></a>Tipo de recurso cloudPC

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma área de trabalho virtual gerenciada pela nuvem. Esse computador cloud também está inscrito no Intune e gerenciado por meio do portal Microsoft Endpoint Manager, portanto, o Cloud PC também tem uma ID de dispositivo gerenciado correspondente do Intune.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[Coleção cloudPC](../resources/cloudpc.md)|Listar propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .|
|[Obter cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Leia as propriedades e as relações de um [objeto cloudPC](../resources/cloudpc.md) .|
|[Alterar o tipo de conta de usuário](../api/cloudpc-changeuseraccounttype.md)|Nenhum|Altere o tipo de conta do usuário em um computador cloud específico.|
|[Fim do período de carência](../api/cloudpc-endgraceperiod.md)|Nenhum|Termine o período de carência para um [objeto cloudPC](../resources/cloudpc.md) .|
|[Obter resultados de ação remota](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Verifique os [resultados da ação remota especificada pelo computador na nuvem](../resources/cloudpcremoteactionresult.md) para um dispositivo cloud pc.|
|[Reiniciar](../api/cloudpc-reboot.md)|Nenhum|Reiniciar um objeto [cloudPC](../resources/cloudpc.md) específico.|
|[Rename](../api/cloudpc-rename.md)|Nenhum|Renomeie um objeto [cloudPC](../resources/cloudpc.md) específico. Use essa API para atualizar **o displayName** para a entidade cloud pc.|
|[Reprovision](../api/cloudpc-reprovision.md)|Nenhum|Reprovisionar um [objeto cloudPC](../resources/cloudpc.md) .|
|[Ação remota de reprovisionamento](../api/manageddevice-reprovisioncloudpc.md)|Nenhum|Reprovisionar um computador cloud com uma ID de dispositivo  [gerenciado do](../resources/cloudpc.md) Intune.|
|[Ação remota de reprovisionamento em massa](../api/manageddevice-bulkreprovisioncloudpc.md)|Nenhum(a)|Reprovisionar em massa um conjunto de dispositivos cloud pc com IDs de dispositivo gerenciado do Intune.|
|[Resize a ação remota](../api/manageddevice-resizecloudpc.md)|Nenhum(a)|Atualize ou downgrade um computador cloud existente para outra configuração com novo vCPU e tamanho de armazenamento por meio da ID do dispositivo gerenciado do Intune.|
|[Solução de problemas](../api/cloudpc-troubleshoot.md)|Nenhum|Solucionar problemas de um [objeto cloudPC](../resources/cloudpc.md) específico. Use essa API para verificar o status de saúde do computador na nuvem e do host da sessão.|
|[Restaurar a ação remota](../api/manageddevice-restorecloudpc.md)|Nenhum|Restaure um dispositivo cloud pc para um estado anterior de um instantâneo.|
|[Ação remota de restauração em massa](../api/manageddevice-bulkrestorecloudpc.md)|[cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md)|Restaure vários dispositivos cloud pc com uma única solicitação que inclui as IDs de dispositivos gerenciados do Intune e uma data e hora de ponto de restauração.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aadDeviceId|Cadeia de caracteres|A Azure Active Directory (Azure AD) do computador cloud.|
|displayName|String|O nome de exibição do Cloud PC.|
|gracePeriodEndDateTime|DateTimeOffset|A data e a hora em que o período de carência termina e o reprovisionamento/desprovisionamento acontece. Obrigatório somente se o status for `inGracePeriod`. O timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|id|String|O identificador exclusivo para o Cloud PC. Somente leitura.|
|imageDisplayName|Cadeia de caracteres|Nome da imagem do sistema operacional que está no cloud pc.|
|lastLoginResult|[cloudPcLoginResult](../resources/cloudpcloginresult.md)|O último resultado de logon do Cloud PC. Por exemplo, `{ "time": "2014-01-01T00:00:00Z"}`.|
|lastModifiedDateTime|DateTimeOffset|A última data e hora modificadas do Cloud PC. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|lastRemoteActionResult|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|O último resultado de ação remota dos PCs de nuvem corporativos. As ações remotas com suporte são: `Reboot`, `Rename`, `Reprovision`, `Restore`e `Troubleshoot`.|
|managedDeviceId|Cadeia de caracteres|A ID do dispositivo Intune do computador cloud.|
|managedDeviceName|String|O nome do dispositivo Intune do Computador na Nuvem.|
|onPremisesConnectionName|String|A conexão local que é aplicada durante o provisionamento de PCs na Nuvem.|
|osVersion|[cloudPcOperatingSystem](../resources/cloudpcorganizationsettings.md#cloudpcoperatingsystem-values)|A versão do sistema operacional (OS) a ser provisionada em PCs na Nuvem. Os valores possíveis são: `windows10`, `windows11`e `unknownFutureValue`.|
|provisioningPolicyId|String|A ID da política de provisionamento do Cloud PC.|
|provisioningPolicyName|String|A política de provisionamento que é aplicada durante o provisionamento de PCs de Nuvem.|
|servicePlanId|String|A ID do plano de serviço do Cloud PC.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviço do Cloud PC.|
|servicePlanType|[cloudPcServicePlanType](../resources/cloudpcserviceplan.md#cloudpcserviceplantype-values)|O tipo de plano de serviço do Cloud PC.|
|status|[cloudPcStatus](#cloudpcstatus-values)|O status do Cloud PC. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`, `restoring`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Os detalhes do status do computador na nuvem.|
|userAccountType|[cloudPcUserAccountType](../resources/cloudpcorganizationsettings.md#cloudpcuseraccounttype-values)|O tipo de conta do usuário em PCs de Nuvem provisionados. Os valores possíveis são: `standardUser`, `administrator`e `unknownFutureValue`.|
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
|pendingProvision|O provisionamento está pendente no Cloud PC. Nesse caso, o número de PCs de Nuvem no período de carência é maior do que o número total de licenças disponíveis. |
|restaurando|O Cloud PC está restaurando.|
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
  "userAccountType": "String",
  "osVersion": "String",
  "lastRemoteActionResult": "String",
  "lastLoginResult": "String"
}
```
