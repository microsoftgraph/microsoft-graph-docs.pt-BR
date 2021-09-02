---
title: Tipo de recurso userExperienceAnalyticsBaseline
description: A entidade de linha de base de análise de experiência do usuário contém valores de linha de base para comparar as pontuações de análise de experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 730537696691c1039e924817d653497fb147338b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803774"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a>Tipo de recurso userExperienceAnalyticsBaseline

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de linha de base de análise de experiência do usuário contém valores de linha de base para comparar as pontuações de análise de experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsBaselines](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|[Coleção userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Obter userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Criar userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Crie um novo [objeto userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|
|[Excluir userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|Nenhum(a)|Exclui um [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).|
|[Atualizar userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da linha de base de análise de experiência do usuário.|
|displayName|Cadeia de caracteres|O nome da linha de base de análise de experiência do usuário.|
|overallScore|Int32|A pontuação geral da linha de base de análise de experiência do usuário.|
|isBuiltIn|Booliano|Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.|
|createdDateTime|DateTimeOffset|A data em que a linha de base personalizada foi criada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|As métricas de desempenho do dispositivo de análise de experiência do usuário.|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|As métricas de práticas recomendadas da análise da experiência do usuário.|
|rebootAnalyticsMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|As métricas de análise de reinicialização da experiência do usuário.|
|resourcePerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|As métricas de desempenho do recurso de análise de experiência do usuário.|
|appHealthMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|As métricas de saúde do aplicativo de análise de experiência do usuário.|
|workFromAnywhereMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|A análise da experiência do usuário funciona de qualquer lugar.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
  "isBuiltIn": true,
  "createdDateTime": "String (timestamp)"
}
```



