---
title: Tipo de recurso windowsUniversalAppXContainedApp
description: Uma classe que representa um aplicativo contido de um aplicativo WindowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 990989d50774622990d88345e24aa7e8a1a9994bd922d53e61bb2d36e339c90c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253142"
---
# <a name="windowsuniversalappxcontainedapp-resource-type"></a>Tipo de recurso windowsUniversalAppXContainedApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que representa um aplicativo contido de um aplicativo WindowsUniversalAppX.


Herda de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsUniversalAppXContainedApps](../api/intune-apps-windowsuniversalappxcontainedapp-list.md)|[Coleção windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Listar propriedades e relações dos [objetos windowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|
|[Obter windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-get.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Leia propriedades e relações do [objeto windowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|
|[Criar windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-create.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Crie um novo [objeto windowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|
|[Excluir windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-delete.md)|Nenhum|Exclui um [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|
|[Atualizar windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-update.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Atualize as propriedades de um [objeto windowsUniversalAppXContainedApp.](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|Cadeia de caracteres|A ID do modelo de usuário do aplicativo contido de um aplicativo WindowsUniversalAppX.|

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




