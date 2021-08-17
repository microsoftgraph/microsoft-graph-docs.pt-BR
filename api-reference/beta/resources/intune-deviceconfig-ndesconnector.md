---
title: Tipo de recurso ndesConnector
description: Entidade que representa um conector OnPrem Ndes.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20f58e58b36abe69ecdb9ef24da990516d8ea01ed37cf3ad3fba44e6f708fdb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54198245"
---
# <a name="ndesconnector-resource-type"></a>Tipo de recurso ndesConnector

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um conector OnPrem Ndes.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|[Coleção ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Listar propriedades e relações dos objetos [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|
|[Obter ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Leia propriedades e relações do [objeto ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|
|[Criar ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Crie um novo [objeto ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|
|[Excluir ndesConnector](../api/intune-deviceconfig-ndesconnector-delete.md)|Nenhum|Exclui um [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|
|[Atualizar ndesConnector](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Atualize as propriedades de um [objeto ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave do Conector NDES.|
|lastConnectionDateTime|DateTimeOffset|Última hora de conexão para o Conector do Ndes|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Status do Conector do Ndes. Os valores possíveis são: `none`, `active`, `inactive`.|
|displayName|Cadeia de caracteres|O nome amigável do Conector do Ndes.|

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




