---
title: tipo de recurso de microsoftStoreForBusinessContainedApp
description: Uma classe que representa um aplicativo contido de um MicrosoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f783475e2f1f49745b29903689e75d854c233352
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876969"
---
# <a name="microsoftstoreforbusinesscontainedapp-resource-type"></a>tipo de recurso de microsoftStoreForBusinessContainedApp

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe que representa um aplicativo contido de um MicrosoftStoreForBusinessApp.

Herda de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista microsoftStoreForBusinessContainedApps](../api/intune-apps-microsoftstoreforbusinesscontainedapp-list.md)|coleção [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|Lista as propriedades e os relacionamentos dos objetos [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .|
|[Obter microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-get.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|Leia as propriedades e os relacionamentos do objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .|
|[Criar microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-create.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|Crie um novo objeto de [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .|
|[Excluir microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-delete.md)|Nenhum|Exclui um [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).|
|[Atualizar microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-update.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|Atualize as propriedades de um objeto [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|Cadeia de caracteres|A ID de modelo de usuário do aplicativo do aplicativo de um MicrosoftStoreForBusinessApp contido.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```





