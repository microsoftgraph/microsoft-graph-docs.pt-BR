---
title: tipo de recurso de outOfBoxExperienceSettings
description: Configuração inicial pelo usuário configuração
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af276dd520df9ee3b257650e703813de355bed9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882730"
---
# <a name="outofboxexperiencesettings-resource-type"></a>tipo de recurso de outOfBoxExperienceSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração inicial pelo usuário configuração
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hidePrivacySettings|Booliano|Mostrar ou ocultar as configurações de privacidade para o usuário|
|hideEULA|Booliano|Mostrar ou ocultar o EULA ao usuário|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Tipo de usuário. Os valores possíveis são: `administrator` e `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|Tipo de autenticação de ingresso AAD. Os valores possíveis são: `singleUser` e `shared`.|
|skipKeyboardSelectionPage|Booliano|Se definido, em seguida, ignore a seleção de teclado página se estiver definida região e idioma|
|hideEscapeLink|Booliano|Se definido como verdadeiro, em seguida, o usuário não pode começar novamente com uma conta diferente, na empresa entrar|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```





