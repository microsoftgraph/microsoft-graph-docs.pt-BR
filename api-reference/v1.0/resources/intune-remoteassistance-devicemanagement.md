---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fcfb85a6147acbf8d8a64d3b80f568f4ac8603ec
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60448952"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-remoteassistance-devicemanagement-get.md)|[deviceManagement](../resources/intune-remoteassistance-devicemanagement.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-remoteassistance-devicemanagement-update.md)|[deviceManagement](../resources/intune-remoteassistance-devicemanagement.md)|Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|remoteAssistancePartners|Conjunto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Os parceiros de assistência remota.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



