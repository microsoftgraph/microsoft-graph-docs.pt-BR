---
title: Tipo de recurso cloudPcServicePlan
description: Representa uma coleção definida de configurações de plano de serviço que os PCs da Nuvem suportam para um locatário.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d2950e65ec3f90f2c7a3e55123e46c435dc805f4
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697176"
---
# <a name="cloudpcserviceplan-resource-type"></a>Tipo de recurso cloudPcServicePlan

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção definida de configurações de plano de serviço que os PCs da Nuvem suportam para um locatário.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar servicePlans](../api/virtualendpoint-list-serviceplans.md)|[Coleção cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Listar os planos de serviço que os PCs de Nuvem suportam para esse locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome do plano de serviço. Somente leitura.|
|id|String|Identificador exclusivo do plano de serviço. Somente leitura.|
|ramInGB|Int32|O tamanho da RAM em GB. Apenas leitura.|
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
