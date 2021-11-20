---
title: Tipo de recurso cloudPcServicePlan
description: Representa um Windows de serviço 365 configurado para um computador cloud.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 281bfdbaefde3b58b8bb9c0367d92d7dfc0bebb3
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123948"
---
# <a name="cloudpcserviceplan-resource-type"></a>Tipo de recurso cloudPcServicePlan

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um Windows de serviço 365 configurado para um computador cloud.

Para exemplos de planos de serviço disponíveis no momento, consulte [Windows 365 comparar planos e preços.](https://www.microsoft.com/windows-365/business/compare-plans-pricing) Atualmente, a API Graph microsoft está disponível para Windows 365 Enterprise.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar servicePlans](../api/virtualendpoint-list-serviceplans.md)|[Coleção cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Lista os planos de serviço disponíveis no momento que a organização pode comprar para os PCs de Nuvem.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome do plano de serviço. Somente leitura.|
|id|Cadeia de caracteres|Identificador exclusivo do plano de serviço. Somente leitura.|
|ramInGB|Int32|O tamanho da RAM em GB. Somente leitura.|
|storageInGB|Int32|O tamanho do disco do sistema operacional em GB. Somente leitura.|
|type|[cloudPcServicePlanType](#cloudpcserviceplantype-values)|O tipo do plano de serviço. Os valores possíveis são: `enterprise`, `business`, `unknownFutureValue`. Somente leitura.|
|userProfileInGB|Int32|O tamanho do disco de perfil do usuário em GB. Somente leitura.|
|vCpuCount|Int32|O número de vCPUs. Somente leitura.|

### <a name="cloudpcserviceplantype-values"></a>Valores cloudPcServicePlanType

|Member|Descrição|
|:---|:---|
|enterprise|Enterprise tipo de plano de serviço para clientes corporativos.|
|business|Tipo de plano de serviço comercial para clientes VSB (Muito Pequenos Negócios).|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcServicePlan",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcServicePlan",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "vCpuCount": "Int32",
  "ramInGB": "Int32",
  "storageInGB": "Int32",
  "userProfileInGB": "Int32"
}
```
