---
title: Tipo de recurso connectionQuota
description: Representa a cota de conexão que contém informações calculadas sobre a utilização da cota de uma conexão externa.
author: snlraju-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 68a8015115157bbc7ca12a9851c7386053e2d72a
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629209"
---
# <a name="connectionquota-resource-type"></a>Tipo de recurso connectionQuota

Namespace: microsoft.graph.externalConnectors

Representa a [cota de](externalconnectors-externalconnection.md) conexão que contém informações calculadas sobre a utilização da cota de uma conexão externa. Ele retorna o número permitido de itens que você pode ingerir em uma conexão considerando os itens ingeridos para a conexão em relação à cota no nível do locatário para conectores do Microsoft Graph.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Obter connectionQuota](../api/externalconnectors-connectionquota-get.md) |[connectionQuota](../resources/externalconnectors-connectionquota.md)| Recupere as propriedades e as relações de uma **connectionQuota**. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| itemsRemaining | Int64 | O mínimo de dois valores, um representando os *itens restantes na conexão e* os outros *itens restantes no nível do locatário*. <br/>A equação a seguir representa a fórmula usada para calcular o número mínimo:<br/> min (\{_&#65279;capacidade_\} máxima na _conexão –_\}\{&#65279;número de itens na _conexão,_\} \{ cota de locatário&#65279;– \{&#65279;número de itens _indexados_ em todas as conexões\}). <br/>Se a conexão não for monetizada, como em um conector de visualização ou experiência de conteúdo de visualização, essa propriedade será simplesmente o número de itens restantes na conexão. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionQuota",
  "openType": false
}
-->

``` json
{
  "itemsRemaining": "Int64"
}
```
