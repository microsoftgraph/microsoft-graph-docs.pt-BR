---
title: tipo de recurso de ndesConnector
description: Entidade que representa um conector OnPrem Ndes.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 582d49ccd9a5d61c144e3ef915994302515dbe40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884914"
---
# <a name="ndesconnector-resource-type"></a>tipo de recurso de ndesConnector

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade que representa um conector OnPrem Ndes.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|coleção [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Lista as propriedades e os relacionamentos dos objetos [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Obter ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Leia as propriedades e os relacionamentos do objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Criar ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Crie um novo objeto de [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Excluir ndesConnector](../api/intune-deviceconfig-ndesconnector-delete.md)|Nenhum|Exclui um [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|
|[Atualizar ndesConnector](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Atualize as propriedades de um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave do conector NDES.|
|lastConnectionDateTime|DateTimeOffset|Hora da última conexão para o conector Ndes|
|estado|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Status do conector NDES. Os valores possíveis são: `none`, `active`, `inactive`.|
|displayName|Cadeia de caracteres|O nome amigável do conector Ndes.|

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





