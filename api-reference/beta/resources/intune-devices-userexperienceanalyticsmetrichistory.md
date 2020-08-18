---
title: tipo de recurso userExperienceAnalyticsMetricHistory
description: O histórico de métrica de análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f9523c747bf6f3c82a7793ec8a60f02109700d7
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793143"
---
# <a name="userexperienceanalyticsmetrichistory-resource-type"></a>tipo de recurso userExperienceAnalyticsMetricHistory

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O histórico de métrica de análise da experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsMetricHistories](../api/intune-devices-userexperienceanalyticsmetrichistory-list.md)|coleção [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .|
|[Obter userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-get.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .|
|[Criar userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-create.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Criar um novo objeto [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .|
|[Excluir userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-delete.md)|Nenhum|Exclui [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).|
|[Atualizar userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-update.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do histórico de métricas de análise da experiência do usuário.|
|metricDateTime|DateTimeOffset|A data e hora da métrica da análise da experiência do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|userExperienceAnalyticsMetric|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Métrica de análise da experiência do usuário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetricHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "String (identifier)",
  "metricDateTime": "String (timestamp)"
}
```



