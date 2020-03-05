---
title: tipo de recurso ndesConnector
description: Entidade que representa um conector NDES local.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1894e9e91f74fdfec2c1531a908b2237d382f8a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526003"
---
# <a name="ndesconnector-resource-type"></a>tipo de recurso ndesConnector

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um conector NDES local.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|coleção [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Listar Propriedades e relações dos objetos [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Obter ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Leia as propriedades e as relações do objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Criar ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Criar um novo objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Excluir ndesConnector](../api/intune-deviceconfig-ndesconnector-delete.md)|Nenhum|Exclui [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|
|[Atualizar ndesConnector](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Atualiza as propriedades de um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave do conector NDES.|
|lastConnectionDateTime|DateTimeOffset|Hora da última conexão para o conector NDES|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Status do conector NDES. Os valores possíveis são: `none`, `active`, `inactive`.|
|displayName|Cadeia de caracteres|O nome amigável do conector NDES.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ndesConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "String (identifier)",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "displayName": "String"
}
```



