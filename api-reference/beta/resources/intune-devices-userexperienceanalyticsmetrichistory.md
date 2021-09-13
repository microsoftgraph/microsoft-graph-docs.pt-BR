---
title: Tipo de recurso userExperienceAnalyticsMetricHistory
description: Histórico métrico da análise da experiência do usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b0d63d65992a1034587b63b96d2c694701de93dc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054363"
---
# <a name="userexperienceanalyticsmetrichistory-resource-type"></a>Tipo de recurso userExperienceAnalyticsMetricHistory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Histórico métrico da análise da experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsMetricHistories](../api/intune-devices-userexperienceanalyticsmetrichistory-list.md)|[coleção userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|
|[Obter userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-get.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|
|[Criar userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-create.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Crie um novo [objeto userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|
|[Excluir userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).|
|[Atualizar userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-update.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do histórico métrico de análise da experiência do usuário.|
|deviceId|Cadeia de caracteres|A ID do dispositivo de análise de experiência do usuário.|
|metricDateTime|DateTimeOffset|A data de data métrica da análise da experiência do usuário.|
|metricType|Cadeia de Caracteres|O tipo métrico de análise de experiência do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|userExperienceAnalyticsMetric|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Métrica de análise de experiência do usuário.|

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
  "deviceId": "String",
  "metricDateTime": "String (timestamp)",
  "metricType": "String"
}
```



