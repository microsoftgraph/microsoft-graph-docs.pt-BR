---
title: Tipo de recurso windowsManagementApp
description: Windows de aplicativo de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 969ffdb3905a0feb1a636a38daf8bcae95630b4c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58807255"
---
# <a name="windowsmanagementapp-resource-type"></a>Tipo de recurso windowsManagementApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows de aplicativo de gerenciamento.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter windowsManagementApp](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Leia propriedades e relações do [objeto windowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)|
|[Atualizar windowsManagementApp](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Atualize as propriedades de um [objeto windowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)|
|[ação setAsManagedInstaller](../api/intune-devices-windowsmanagementapp-setasmanagedinstaller.md)|Nenhum(a)|Definir o status do Instalador Gerenciado para o locatário do chamador|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do aplicativo Windows de gerenciamento|
|availableVersion|Cadeia de caracteres|Windows versão disponível do aplicativo de gerenciamento.|
|managedInstaller|[managedInstallerStatus](../resources/intune-devices-managedinstallerstatus.md)|Status do Instalador Gerenciado. Os valores possíveis são: `disabled` e `enabled`.|
|managedInstallerConfiguredDateTime|Cadeia de caracteres|Data configurada do Instalador Gerenciado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|healthStates|[coleção windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|A lista de estados de saúde para o aplicativo de gerenciamento Windows instalado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String",
  "managedInstaller": "String",
  "managedInstallerConfiguredDateTime": "String"
}
```



