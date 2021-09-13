---
title: Tipo de recurso userExperienceAnalyticsMetric
description: A métrica de análise de experiência do usuário contém a pontuação e unidades de uma métrica de uma categoria de anlaytics de experiência do usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 352a89293bb38e7f03bd7e83d003d465d052335b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125698"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a>Tipo de recurso userExperienceAnalyticsMetric

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A métrica de análise de experiência do usuário contém a pontuação e unidades de uma métrica de uma categoria de anlaytics de experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsMetrics](../api/intune-devices-userexperienceanalyticsmetric-list.md)|[Coleção userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)|
|[Obter userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Ler propriedades e relações do [objeto userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)|
|[Criar userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-create.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Crie um novo [objeto userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)|
|[Excluir userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).|
|[Atualizar userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da métrica de análise de experiência do usuário.|
|valor|Duplo|O valor da métrica de análise da experiência do usuário.|
|unidade|Cadeia de Caracteres|A unidade da métrica de análise de experiência do usuário.|

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



