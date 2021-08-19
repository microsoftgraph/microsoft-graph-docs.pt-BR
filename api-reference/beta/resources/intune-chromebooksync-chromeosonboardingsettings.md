---
title: Tipo de recurso chromeOSOnboardingSettings
description: Entidade que representa as configurações de locatário do Chromebook
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53b42eae58cbd68f4663290cd5d565e8fdf44c27bab676835054dcbc919a8935
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206785"
---
# <a name="chromeosonboardingsettings-resource-type"></a>Tipo de recurso chromeOSOnboardingSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa as configurações de locatário do Chromebook

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar chromeOSOnboardingSettingses](../api/intune-chromebooksync-chromeosonboardingsettings-list.md)|[Coleção chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|Listar propriedades e relações dos [objetos chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|
|[Obter chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-get.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|Leia propriedades e relações do [objeto chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|
|[Criar chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-create.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|Crie um novo [objeto chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|
|[Excluir chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-delete.md)|Nenhum|Exclui um [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md).|
|[Atualizar chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-update.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|Atualize as propriedades de um [objeto chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|
|[ação connect](../api/intune-chromebooksync-chromeosonboardingsettings-connect.md)|[chromeOSOnboardingStatus](../resources/intune-chromebooksync-chromeosonboardingstatus.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do ChromebookTenant|
|ownerUserPrincipalName|String|OwnerUserPrincipalName do ChromebookTenant|
|onboardingStatus|[onboardingStatus](../resources/intune-chromebooksync-onboardingstatus.md)|OnboardingStatus do ChromebookTenant. Os valores possíveis são: `unknown`, `inprogress`, `onboarded`, `failed`.|
|lastModifiedDateTime|DateTimeOffset|LastModifiedDateTime do ChromebookTenant|
|lastDirectorySyncDateTime|DateTimeOffset|LastDirectorySyncDateTime do ChromebookTenant|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chromeOSOnboardingSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "id": "String (identifier)",
  "ownerUserPrincipalName": "String",
  "onboardingStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastDirectorySyncDateTime": "String (timestamp)"
}
```




