---
title: Tipo de recurso mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 281100ad8f91bc8872cba5228a1d6a9a24a42167
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075841"
---
# <a name="mobilecontainedapp-resource-type"></a>Tipo de recurso mobileContainedApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[Coleção mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Listar propriedades e relações dos objetos [mobileContainedApp.](../resources/intune-apps-mobilecontainedapp.md)|
|[Obter mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Leia propriedades e relações do [objeto mobileContainedApp.](../resources/intune-apps-mobilecontainedapp.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|

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



