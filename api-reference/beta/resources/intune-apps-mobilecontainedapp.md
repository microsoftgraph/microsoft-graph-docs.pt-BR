---
title: tipo de recurso de mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.
ms.openlocfilehash: abd47e8e9449a111c212d20b4f867a9064f612e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037424"
---
# <a name="mobilecontainedapp-resource-type"></a>tipo de recurso de mobileContainedApp

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Lista as propriedades e os relacionamentos dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .|
|[Obter mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Leia as propriedades e os relacionamentos do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```





