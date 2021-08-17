---
title: tipo de recurso userExperienceAnalyticsAppHealthOSVersionPerformance
description: A entidade de desempenho da versão do sistema operacional do dispositivo de análise de experiência do usuário contém detalhes de desempenho da versão do sistema operacional.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d6d43ad592821546c9eab32c3681ae7ab9747def7fe71c18b72ef579f4c3bb28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54133212"
---
# <a name="userexperienceanalyticsapphealthosversionperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthOSVersionPerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho da versão do sistema operacional do dispositivo de análise de experiência do usuário contém detalhes de desempenho da versão do sistema operacional.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthOSVersionPerformances](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-list.md)|[coleção userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|
|[Obter userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-get.md)|[userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|
|[Criar userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-create.md)|[userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Crie um novo [objeto userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|
|[Excluir userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md).|
|[Atualizar userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-update.md)|[userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho de versão do sistema operacional de análise de experiência do usuário.|
|osVersion|String|A versão do sistema operacional instalada no dispositivo.|
|osBuildNumber|Cadeia de caracteres|O número de com build do sistema operacional instalado no dispositivo.|
|activeDeviceCount|Int32|O número de dispositivos ativos para a versão do sistema operacional. Valores válidos -2147483648 para 2147483647|
|meanTimeToFailureInMinutes|Int32|O tempo de falha média para a versão do sistema operacional em minutos. Valores válidos -2147483648 para 2147483647|
|osVersionAppHealthScore|Duplo|A pontuação de saúde do aplicativo da versão do sistema operacional. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|osVersionAppHealthStatus|Cadeia de caracteres|O status geral da saúde do aplicativo da versão do sistema operacional.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "id": "String (identifier)",
  "osVersion": "String",
  "osBuildNumber": "String",
  "activeDeviceCount": 1024,
  "meanTimeToFailureInMinutes": 1024,
  "osVersionAppHealthScore": "4.2",
  "osVersionAppHealthStatus": "String"
}
```




