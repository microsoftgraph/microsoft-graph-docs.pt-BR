---
title: Tipo de recurso remoteAssistanceSettings
description: Configurações de assistência remota para a conta
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7eebfdcef7a3da9558ce51eeac88d58c2a79c692
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58263327"
---
# <a name="remoteassistancesettings-resource-type"></a>Tipo de recurso remoteAssistanceSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configurações de assistência remota para a conta

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter remoteAssistanceSettings](../api/intune-remoteassistance-remoteassistancesettings-get.md)|[remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md)|Leia propriedades e relações do [objeto remoteAssistanceSettings.](../resources/intune-remoteassistance-remoteassistancesettings.md)|
|[Atualizar remoteAssistanceSettings](../api/intune-remoteassistance-remoteassistancesettings-update.md)|[remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md)|Atualize as propriedades de [um objeto remoteAssistanceSettings.](../resources/intune-remoteassistance-remoteassistancesettings.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de configurações de assistência remota|
|remoteAssistanceState|[remoteAssistanceState](../resources/intune-remoteassistance-remoteassistancestate.md)|O estado atual da assistência remota para a conta. Os valores possíveis são: notConfigured, disabled, enabled. Essa configuração é configurável pelo administrador. As configurações de assistência remota que ainda não foram configuradas pelo administrador têm um estado nãoConfigurado. Retornado por padrão. Os valores possíveis são: `notConfigured`, `disabled`, `enabled`.|
|allowSessionsToUnenrolledDevices|Boolean| Indica se as sessões para dispositivos não reemrollados são permitidas para a conta. Essa configuração é configurável pelo administrador. O valor padrão é false.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistanceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistanceSettings",
  "id": "String (identifier)",
  "remoteAssistanceState": "String",
  "allowSessionsToUnenrolledDevices": true
}
```




