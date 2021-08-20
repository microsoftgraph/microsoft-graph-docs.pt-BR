---
title: Tipo de recurso mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 47dc0c867487c4043f148d8f3469288b7c0dc5d4d119a1eda412f99ad983c1c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54156461"
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




