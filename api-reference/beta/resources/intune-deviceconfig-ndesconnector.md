---
title: tipo de recurso ndesConnector
description: Entidade que representa um conector NDES local.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 36d41032e98253f81a409665fb35b7e25f672053
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273323"
---
# <a name="ndesconnector-resource-type"></a>tipo de recurso ndesConnector

Namespace: microsoft.graph

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
|displayName|String|O nome amigável do conector NDES.|

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




