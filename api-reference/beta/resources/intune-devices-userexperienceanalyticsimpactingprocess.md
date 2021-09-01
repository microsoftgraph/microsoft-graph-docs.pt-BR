---
title: Tipo de recurso userExperienceAnalyticsImpactingProcess
description: A entidade de processo de análise de experiência do usuário principal que afeta.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fe90734826416aca89065c47568ce9e68d085753
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794403"
---
# <a name="userexperienceanalyticsimpactingprocess-resource-type"></a>Tipo de recurso userExperienceAnalyticsImpactingProcess

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de processo de análise de experiência do usuário principal que afeta.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsImpactingProcesses](../api/intune-devices-userexperienceanalyticsimpactingprocess-list.md)|[Coleção userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|
|[Obter userExperienceAnalyticsImpactingProcess](../api/intune-devices-userexperienceanalyticsimpactingprocess-get.md)|[userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|
|[Criar userExperienceAnalyticsImpactingProcess](../api/intune-devices-userexperienceanalyticsimpactingprocess-create.md)|[userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|Crie um novo [objeto userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|
|[Excluir userExperienceAnalyticsImpactingProcess](../api/intune-devices-userexperienceanalyticsimpactingprocess-delete.md)|Nenhum(a)|Exclui um [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md).|
|[Atualizar userExperienceAnalyticsImpactingProcess](../api/intune-devices-userexperienceanalyticsimpactingprocess-update.md)|[userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da entidade de processo de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo afetado.|
|category|Cadeia de caracteres|A categoria do processo de impacto.|
|processName|Cadeia de caracteres|O nome do processo.|
|descrição|Cadeia de caracteres|A descrição do processo.|
|publicador|String|O editor do processo.|
|impactValue|Duplo|O valor de impacto do processo. Valores válidos de 0 a 1,79769313486232E+308|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsImpactingProcess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "id": "String (identifier)",
  "deviceId": "String",
  "category": "String",
  "processName": "String",
  "description": "String",
  "publisher": "String",
  "impactValue": "4.2"
}
```



