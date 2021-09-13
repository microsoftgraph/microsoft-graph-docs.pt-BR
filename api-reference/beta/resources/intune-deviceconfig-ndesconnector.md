---
title: Tipo de recurso ndesConnector
description: Entidade que representa um conector OnPrem Ndes.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 222c675d66fc400c83161377def32420ad81d3fa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091647"
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



