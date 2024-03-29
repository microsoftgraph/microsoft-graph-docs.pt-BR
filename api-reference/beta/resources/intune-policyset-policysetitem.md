---
title: Tipo de recurso policySetItem
description: Uma classe que contém as propriedades usadas para Item PolicySet.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05647e77adc9c6d0b9b65cebbdf2c2890c10e0c5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074854"
---
# <a name="policysetitem-resource-type"></a>Tipo de recurso policySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para Item PolicySet.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar policySetItems](../api/intune-policyset-policysetitem-list.md)|[Coleção policySetItem](../resources/intune-policyset-policysetitem.md)|Listar propriedades e relações dos [objetos policySetItem.](../resources/intune-policyset-policysetitem.md)|
|[Obter policySetItem](../api/intune-policyset-policysetitem-get.md)|[policySetItem](../resources/intune-policyset-policysetitem.md)|Leia propriedades e relações do [objeto policySetItem.](../resources/intune-policyset-policysetitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do PolicySetItem.|
|createdDateTime|DateTimeOffset|Hora de criação do PolicySetItem.|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do PolicySetItem.|
|payloadId|Cadeia de caracteres|PayloadId do PolicySetItem.|
|itemType|Cadeia de caracteres|policySetType do PolicySetItem.|
|displayName|Cadeia de caracteres|DisplayName do PolicySetItem.|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status do PolicySetItem. Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro se ocorrer algum. Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Conjunto de cadeias de caracteres|Marcas da implantação guiada|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```



