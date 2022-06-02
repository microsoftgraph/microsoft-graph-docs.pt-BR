---
title: Tipo de recurso userExperienceAnalyticsDeviceScope
description: A entidade de escopo do dispositivo de análise de experiência do usuário contém valores de configuração de escopo do dispositivo usados para aplicar a filtragem nos relatórios de análise de ponto de extremidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf5605a0f65dcf4e4d35026bf18d5499ab2a6c96
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858494"
---
# <a name="userexperienceanalyticsdevicescope-resource-type"></a>Tipo de recurso userExperienceAnalyticsDeviceScope

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de escopo do dispositivo de análise de experiência do usuário contém valores de configuração de escopo do dispositivo usados para aplicar a filtragem nos relatórios de análise de ponto de extremidade.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsDeviceScopes](../api/intune-devices-userexperienceanalyticsdevicescope-list.md)|[coleção userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .|
|[Obter userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-get.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|Leia as propriedades e as relações do [objeto userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .|
|[Criar userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-create.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|Crie um [novo objeto userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .|
|[Excluir userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md).|
|[Atualizar userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-update.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .|
|[Ação triggerDeviceScopeAction](../api/intune-devices-userexperienceanalyticsdevicescope-triggerdevicescopeaction.md)|[deviceScopeActionResult](../resources/intune-devices-devicescopeactionresult.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo para a configuração de escopo do dispositivo.|
|deviceScopeName|String|O nome da configuração de escopo do dispositivo de análise de experiência do usuário.|
|ownerId|String|O identificador exclusivo da pessoa (administrador) que criou a configuração de escopo do dispositivo.|
|isBuiltIn|Booliano|Indica se a configuração de escopo do dispositivo é interna ou personalizada. Quando TRUE, a configuração de escopo do dispositivo é interna. Quando FALSE, a configuração de escopo do dispositivo é personalizada. O valor padrão é FALSE.|
|enabled|Boolean|Indica se um escopo de dispositivo está habilitado ou desabilitado. Quando TRUE, o escopo do dispositivo é habilitado. Quando FALSE, o escopo do dispositivo é desabilitado. O valor padrão é FALSE.|
|status|[deviceScopeStatus](../resources/intune-devices-devicescopestatus.md)|Indica o status do escopo do dispositivo depois que o escopo do dispositivo foi habilitado. Os valores possíveis são: none, computing, insufficientData ou completed. O valor padrão é none. Os valores possíveis são: `none`, `computing`, `insufficientData`, `completed`, `unknownFutureValue`.|
|parâmetro|[deviceScopeParameter](../resources/intune-devices-devicescopeparameter.md)|Parâmetro de configuração do escopo do dispositivo. Ele será estendido no futuro para adicionar mais parâmetros. Por exemplo: o parâmetro de escopo do dispositivo pode ser versão do sistema operacional, Tipo de Disco, Fabricante do dispositivo, modelo de dispositivo ou marca de escopo. Valor padrão: scopeTag. Os valores possíveis são: `none`, `scopeTag`, `unknownFutureValue`.|
|operator|[deviceScopeOperator](../resources/intune-devices-devicescopeoperator.md)|Operador de consulta de configuração do escopo do dispositivo. Os valores possíveis são: equals, notEquals, contains, notContains, greaterThan, lessThan. Valor padrão: igual a. Os valores possíveis são: `none`, `equals`, `unknownFutureValue`.|
|valueObjectId|String|O identificador exclusivo para uma ID de marca de escopo de dispositivo de usuário usada para a criação da configuração de escopo do dispositivo.|
|value|Cadeia de caracteres|O valor da cláusula de consulta de configuração do escopo do dispositivo.|
|createdDateTime|DateTimeOffset|Indica a data e a hora de criação para o escopo do dispositivo personalizado.|
|lastModifiedDateTime|DateTimeOffset|Indica a data e a hora da última atualização para o escopo do dispositivo personalizado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScope",
  "id": "String (identifier)",
  "deviceScopeName": "String",
  "ownerId": "String",
  "isBuiltIn": true,
  "enabled": true,
  "status": "String",
  "parameter": "String",
  "operator": "String",
  "valueObjectId": "String",
  "value": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




