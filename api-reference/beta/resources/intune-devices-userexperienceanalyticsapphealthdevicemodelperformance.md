---
title: tipo de recurso userExperienceAnalyticsAppHealthDeviceModelPerformance
description: A entidade de desempenho do modelo de dispositivo de análise de experiência do usuário contém detalhes de desempenho do modelo de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b554ff9ecf59de0486ffb9fc38b360e30ee968b8b6018d60f6b2fcd0590594b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239271"
---
# <a name="userexperienceanalyticsapphealthdevicemodelperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthDeviceModelPerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do modelo de dispositivo de análise de experiência do usuário contém detalhes de desempenho do modelo de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthDeviceModelPerformances](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-list.md)|[coleção userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|
|[Obter userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-get.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|
|[Criar userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-create.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Crie um novo [objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|
|[Excluir userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).|
|[Atualizar userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-update.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho do modelo de dispositivo de análise de experiência do usuário.|
|deviceModel|Cadeia de caracteres|O nome do modelo do dispositivo.|
|deviceManufacturer|Cadeia de caracteres|O nome do fabricante do dispositivo.|
|activeDeviceCount|Int32|O número de dispositivos ativos para o modelo. Valores válidos -2147483648 para 2147483647|
|meanTimeToFailureInMinutes|Int32|O tempo de falha média para o dispositivo modelo em minutos. Valores válidos -2147483648 para 2147483647|
|modelAppHealthScore|Duplo|A pontuação de saúde do aplicativo do modelo de dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|modelAppHealthStatus|Cadeia de caracteres|O status geral da saúde do aplicativo do modelo de dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "id": "String (identifier)",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "activeDeviceCount": 1024,
  "meanTimeToFailureInMinutes": 1024,
  "modelAppHealthScore": "4.2",
  "modelAppHealthStatus": "String"
}
```




