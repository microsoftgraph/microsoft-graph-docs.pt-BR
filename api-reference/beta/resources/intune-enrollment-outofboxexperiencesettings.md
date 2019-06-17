---
title: tipo de recurso outOfBoxExperienceSettings
description: Configuração de experiência inicial da caixa
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92a7e8e2a65817ff6aa144deaa408978804ed963
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963524"
---
# <a name="outofboxexperiencesettings-resource-type"></a>tipo de recurso outOfBoxExperienceSettings

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de experiência inicial da caixa

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hidePrivacySettings|Booliano|Mostrar ou ocultar as configurações de privacidade para o usuário|
|hideEULA|Booliano|Mostrar ou ocultar o EULA para o usuário|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Tipo de usuário. Os valores possíveis são: `administrator` e `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|Tipo de autenticação do AAD join. Os valores possíveis são: `singleUser` e `shared`.|
|skipKeyboardSelectionPage|Booliano|Se definido, ignore a página de seleção de teclado se idioma e região estiverem definidos|
|hideEscapeLink|Booliano|Se for definido como true, o usuário não poderá iniciar novamente com uma conta diferente, na entrada da empresa|

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





