---
title: Tipo de recurso outOfBoxExperienceSettings
description: Configuração de experiência in-locar
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 229564ad320b2d2a2dfce92f1979d23ca12acda6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787565"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Tipo de recurso outOfBoxExperienceSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de experiência in-locar

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hidePrivacySettings|Boleano|Mostrar ou ocultar configurações de privacidade para o usuário|
|hideEULA|Boleano|Mostrar ou ocultar o EULA para o usuário|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Tipo de usuário. Os valores possíveis são: `administrator` e `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|Tipo de autenticação de junção do AAD. Os valores possíveis são: `singleUser` e `shared`.|
|skipKeyboardSelectionPage|Boleano|Se definido, ignore a página de seleção do teclado se Idioma e Região estão definidos|
|hideEscapeLink|Boleano|Se for definido como true, o usuário não poderá começar de novo com uma conta diferente, na assinatura da empresa|

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



