---
title: Tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails
description: A entidade de desempenho do aplicativo de análise de experiência do usuário contém o desempenho do aplicativo por detalhes da versão do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 50962e78755687535c1c696488de13dc19cdc489
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788448"
---
# <a name="userexperienceanalyticsapphealthappperformancebyappversiondetails-resource-type"></a>Tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do aplicativo de análise de experiência do usuário contém o desempenho do aplicativo por detalhes da versão do aplicativo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetailses](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-list.md)|[coleção userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|
|[Obter userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|
|[Criar userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|Crie um novo [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|
|[Excluir userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-delete.md)|Nenhum(a)|Exclui um [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md).|
|[Atualizar userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho do aplicativo de análise de experiência do usuário.|
|deviceCountWithCrashes|Int32|O número total de dispositivos que relataram falhas de um ou mais aplicativos para este aplicativo e versão. Valores válidos -2147483648 para 2147483647|
|isMostUsedVersion|Boleano|É a versão do aplicativo a versão mais usada para esse aplicativo.|
|isLatestUsedVersion|Booliano|É a versão do aplicativo a versão mais recente para esse aplicativo que está em uso.|
|appName|Cadeia de caracteres|O nome do aplicativo.|
|appDisplayName|Cadeia de caracteres|O nome amigável do aplicativo.|
|appPublisher|Cadeia de caracteres|O editor do aplicativo.|
|appVersion|Cadeia de caracteres|A versão do aplicativo.|
|appCrashCount|Int32|O número de falhas para o aplicativo. Valores válidos -2147483648 para 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails",
  "id": "String (identifier)",
  "deviceCountWithCrashes": 1024,
  "isMostUsedVersion": true,
  "isLatestUsedVersion": true,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appVersion": "String",
  "appCrashCount": 1024
}
```



