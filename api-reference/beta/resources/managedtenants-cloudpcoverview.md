---
title: Tipo de recurso cloudPcOverview
description: Representa uma visão geral dos PCs de nuvem para um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a527dea18db31c8d7598a5b04ba538fa9a5af1ab
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401944"
---
# <a name="cloudpcoverview-resource-type"></a>Tipo de recurso cloudPcOverview

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma visão geral dos PCs de nuvem para um determinado locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPcOverviews](../api/managedtenants-managedtenant-list-cloudpcsoverview.md)|[coleção microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md)|Obter uma lista dos objetos [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) e suas propriedades.|
|[Obter cloudPcOverview](../api/managedtenants-cloudpcoverview-get.md)|[microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md)|Leia as propriedades e as relações de um [objeto cloudPcOverview.](../resources/managedtenants-cloudpcoverview.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo para a visão geral do computador na nuvem. Obrigatório. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|numberOfCloudPcConnectionStatusFailed|Int32|O número de conexões de computador na nuvem que têm um status `failed` de . Opcional. Somente leitura.|
|numberOfCloudPcConnectionStatusPassed|Int32|O número de conexões de computador na nuvem que têm um status `passed` de . Opcional. Somente leitura.|
|numberOfCloudPcConnectionStatusPending|Int32|O número de conexões de computador na nuvem que têm um status `pending` de . Opcional. Somente leitura.|
|numberOfCloudPcConnectionStatusRunning|Int32|O número de conexões de computador na nuvem que têm um status `running` de . Opcional. Somente leitura.|
|numberOfCloudPcConnectionStatusUnkownFutureValue|Int32|O número de conexões de computador na nuvem que têm um status `unknownFutureValue` de . Opcional. Somente leitura.|
|numberOfCloudPcStatusDeprovisioning|Int32|O número de PCs de nuvem que têm um status `deprovisioning` de . Opcional. Somente leitura.|
|numberOfCloudPcStatusFailed|Int32|O número de PCs de nuvem que têm um status `failed` de . Opcional. Somente leitura.|
|numberOfCloudPcStatusInGracePeriod|Int32|O número de PCs de nuvem que têm um status `inGracePeriod` de . Opcional. Somente leitura.|
|numberOfCloudPcStatusNotProvisioned|Int32|O número de PCs de nuvem que têm um status `notProvisioned` de . Opcional. Somente leitura.|
|numberOfCloudPcStatusProvisioned|Int32|O número de PCs de nuvem que têm um status `provisioned` de . Opcional. Somente leitura.|
|numberOfCloudPcStatusProvisioning|Int32|O número de PCs de nuvem que têm um status `provisioning` de . Opcional. Somente leitura.|
|numberOfCloudPcStatusUnknown|Int32|O número de PCs de nuvem que têm um status `unknown` de . Opcional. Somente leitura.|
|numberOfCloudPcStatusUpgrading|Int32|O número de PCs de nuvem que têm um status `upgrading` de . Opcional. Somente leitura.|
|tenantDisplayName|Cadeia de caracteres|O nome de exibição do locatário gerenciado. Opcional. Somente leitura.|
|totalCloudPcConnectionStatus|Int32|O número total de status de conexão de computador na nuvem para o locatário gerenciado determinado. Opcional. Somente leitura.|
|totalCloudPcStatus|Int32|O número total de estatuetas de computador na nuvem para o locatário gerenciado determinado. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcOverview",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcOverview",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "totalCloudPcStatus": "Integer",
  "numberOfCloudPcStatusNotProvisioned": "Integer",
  "numberOfCloudPcStatusProvisioning": "Integer",
  "numberOfCloudPcStatusProvisioned": "Integer",
  "numberOfCloudPcStatusUpgrading": "Integer",
  "numberOfCloudPcStatusInGracePeriod": "Integer",
  "numberOfCloudPcStatusDeprovisioning": "Integer",
  "numberOfCloudPcStatusFailed": "Integer",
  "numberOfCloudPcStatusUnknown": "Integer",
  "totalCloudPcConnectionStatus": "Integer",
  "numberOfCloudPcConnectionStatusPending": "Integer",
  "numberOfCloudPcConnectionStatusRunning": "Integer",
  "numberOfCloudPcConnectionStatusPassed": "Integer",
  "numberOfCloudPcConnectionStatusFailed": "Integer",
  "numberOfCloudPcConnectionStatusUnkownFutureValue": "Integer",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
