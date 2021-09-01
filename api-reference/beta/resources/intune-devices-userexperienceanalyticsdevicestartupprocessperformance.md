---
title: Tipo de recurso userExperienceAnalyticsDeviceStartupProcessPerformance
description: O desempenho do processo de inicialização do dispositivo de análise de experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b81d1787bab950011633542653ab0afc81e3883
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794424"
---
# <a name="userexperienceanalyticsdevicestartupprocessperformance-resource-type"></a>Tipo de recurso userExperienceAnalyticsDeviceStartupProcessPerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O desempenho do processo de inicialização do dispositivo de análise de experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsDeviceStartupProcessPerformances](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-list.md)|[coleção userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|
|[Obter userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-get.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|
|[Criar userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-create.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Crie um novo [objeto userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|
|[Excluir userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-delete.md)|Nenhum(a)|Exclui um [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).|
|[Atualizar userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-update.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do desempenho do processo de inicialização do dispositivo de análise de experiência do usuário.|
|processName|Cadeia de caracteres|Nome do processo de inicialização do dispositivo de análise de experiência do usuário.|
|productName|Cadeia de caracteres|O nome do produto do processo de inicialização do dispositivo de análise de experiência do usuário.|
|publicador|String|O editor de processo de inicialização do dispositivo de análise de experiência do usuário.|
|deviceCount|Int64|Contagem resumida do processo de inicialização do dispositivo de análise de experiência do usuário.|
|medianImpactInMs|Int32|Impacto mediano do processo de inicialização do dispositivo de análise da experiência do usuário em milissegundos.|
|totalImpactInMs|Int32|Impacto total do processo de inicialização do dispositivo de análise de experiência do usuário em milissegundos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "id": "String (identifier)",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "deviceCount": 1024,
  "medianImpactInMs": 1024,
  "totalImpactInMs": 1024
}
```



