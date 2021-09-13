---
title: Tipo de recurso hasPayloadLinkResultItem
description: Uma classe que contém o resultado da ação HasPayloadLinks.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad490d3d9574fa42f9dddb4c3bba92934b02287d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080755"
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
|hasLink|Boolean|Indica se uma carga tem um link ou não.|
|erro|Cadeia de Caracteres|As informações de exceção indicam se a verificação desse item foi bem-sucedida ou não. Cadeia de caracteres vazia para nenhum erro.|
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



