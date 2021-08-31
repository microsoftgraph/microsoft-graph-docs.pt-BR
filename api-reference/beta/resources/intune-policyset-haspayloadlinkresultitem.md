---
title: Tipo de recurso hasPayloadLinkResultItem
description: Uma classe que contém o resultado da ação HasPayloadLinks.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 123177d4935ea7aec924345d27134f7ad779a625
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785686"
---
# <a name="haspayloadlinkresultitem-resource-type"></a>Tipo de recurso hasPayloadLinkResultItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém o resultado da ação HasPayloadLinks.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|payloadId|Cadeia de caracteres|Chave da carga, no formato guid.|
|hasLink|Boleano|Indica se uma carga tem um link ou não.|
|erro|Cadeia de caracteres|As informações de exceção indicam se a verificação desse item foi bem-sucedida ou não. Cadeia de caracteres vazia para nenhum erro.|
|fontes|[Coleção deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|O motivo de onde o link vem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hasPayloadLinkResultItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hasPayloadLinkResultItem",
  "payloadId": "String",
  "hasLink": true,
  "error": "String",
  "sources": [
    "String"
  ]
}
```



