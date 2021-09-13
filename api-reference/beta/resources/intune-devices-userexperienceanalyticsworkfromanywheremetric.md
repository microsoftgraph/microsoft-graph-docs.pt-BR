---
title: Tipo de recurso userExperienceAnalyticsWorkFromAnywhereMetric
description: A métrica de análise de experiência do usuário para trabalho de qualquer relatório
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7751ff4575032a4caa63c94f1e8e5c0616b0f4a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101237"
---
# <a name="userexperienceanalyticsworkfromanywheremetric-resource-type"></a>Tipo de recurso userExperienceAnalyticsWorkFromAnywhereMetric

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A métrica de análise de experiência do usuário para trabalho de qualquer relatório

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsWorkFromAnywhereMetrics](../api/intune-devices-userexperienceanalyticsworkfromanywheremetric-list.md)|[coleção userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)|
|[Obter userExperienceAnalyticsWorkFromAnywhereMetric](../api/intune-devices-userexperienceanalyticsworkfromanywheremetric-get.md)|[userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)|
|[Criar userExperienceAnalyticsWorkFromAnywhereMetric](../api/intune-devices-userexperienceanalyticsworkfromanywheremetric-create.md)|[userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)|Crie um novo [objeto userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)|
|[Excluir userExperienceAnalyticsWorkFromAnywhereMetric](../api/intune-devices-userexperienceanalyticsworkfromanywheremetric-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md).|
|[Atualizar userExperienceAnalyticsWorkFromAnywhereMetric](../api/intune-devices-userexperienceanalyticsworkfromanywheremetric-update.md)|[userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da análise de experiência do usuário funciona em qualquer lugar.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|metricDevices|[Coleção userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|O trabalho de dispositivos métricos em qualquer lugar.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric",
  "id": "String (identifier)"
}
```



