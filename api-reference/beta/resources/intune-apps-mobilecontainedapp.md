---
title: tipo de recurso mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 73536b8e1343d2c69296ca7c8149f4fad0e9a34b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491327"
---
# <a name="mobilecontainedapp-resource-type"></a>tipo de recurso mobileContainedApp

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Listar Propriedades e relações dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .|
|[Obter mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Leia as propriedades e as relações do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .|

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



