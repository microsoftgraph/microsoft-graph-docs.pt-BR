---
title: tipo de recurso de windowsUniversalAppXContainedApp
description: Uma classe que representa um aplicativo contido de um aplicativo de WindowsUniversalAppX.
author: tfitzmac
ms.openlocfilehash: 19afa6a677d51613b6a4a18368c53cc5a12a4df7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360141"
---
# <a name="windowsuniversalappxcontainedapp-resource-type"></a>tipo de recurso de windowsUniversalAppXContainedApp

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe que representa um aplicativo contido de um aplicativo de WindowsUniversalAppX.

Herda de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsUniversalAppXContainedApps](../api/intune-apps-windowsuniversalappxcontainedapp-list.md)|coleção [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Lista as propriedades e os relacionamentos dos objetos [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .|
|[Obter windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-get.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Leia as propriedades e os relacionamentos do objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .|
|[Criar windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-create.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Crie um novo objeto de [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .|
|[Excluir windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-delete.md)|Nenhum|Exclui um [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|
|[Atualizar windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-update.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Atualize as propriedades de um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|String|A ID de modelo de usuário do aplicativo do aplicativo de um aplicativo WindowsUniversalAppX contido.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppXContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```





