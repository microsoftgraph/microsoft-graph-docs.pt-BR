---
title: Tipo de recurso outOfBoxExperienceSettings
description: Configuração de experiência in-locar
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed86fd6c8d267aa6f12beb5404b9f7a398fb8f4192ad659580dde8c4734443cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239270"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Tipo de recurso outOfBoxExperienceSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de experiência in-locar

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hidePrivacySettings|Boolean|Mostrar ou ocultar configurações de privacidade para o usuário|
|hideEULA|Boolean|Mostrar ou ocultar o EULA para o usuário|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Tipo de usuário. Os valores possíveis são: `administrator` e `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|Tipo de autenticação de junção do AAD. Os valores possíveis são: `singleUser` e `shared`.|
|skipKeyboardSelectionPage|Boolean|Se definido, ignore a página de seleção do teclado se Idioma e Região estão definidos|
|hideEscapeLink|Boolean|Se for definido como true, o usuário não poderá começar de novo com uma conta diferente, na assinatura da empresa|

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




