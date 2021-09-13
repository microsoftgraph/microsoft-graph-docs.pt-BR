---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton de gerenciamento de aplicativos do dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d88fc5b27d0abc622891d03f3dc5bcd36309fd84
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072026"
---
# <a name="deviceappmanagement-resource-type"></a>Tipo de recurso deviceAppManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton de gerenciamento de aplicativos do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceAppManagement](../api/intune-partnerintegration-deviceappmanagement-get.md)|[deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md)|Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).|
|[Atualizar deviceAppManagement](../api/intune-partnerintegration-deviceappmanagement-update.md)|[deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md)|Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




