---
title: tipo de recurso userExperienceAnalyticsMetric
description: A métrica de análise da experiência do usuário contém a pontuação e as unidades de uma métrica de uma categoria de experiência do usuário Anlaytics.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b44bcb98e642920c5e9bf7804aa9b3790b6228c8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226381"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a>tipo de recurso userExperienceAnalyticsMetric

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A métrica de análise da experiência do usuário contém a pontuação e as unidades de uma métrica de uma categoria de experiência do usuário Anlaytics.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsMetrics](../api/intune-devices-userexperienceanalyticsmetric-list.md)|coleção [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .|
|[Obter userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .|
|[Criar userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-create.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Criar um novo objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .|
|[Excluir userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-delete.md)|Nenhum|Exclui [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).|
|[Atualizar userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da métrica de análise da experiência do usuário.|
|valor|Duplo|O valor da métrica de análise da experiência do usuário.|
|unidade|String|A unidade da métrica de análise da experiência do usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetric"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "String (identifier)",
  "value": "4.2",
  "unit": "String"
}
```




