---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton de gerenciamento de aplicativos do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b88808ea196b0e3cfd75b4845973a377b1a9943b54659b654374a2c87e80fde8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169484"
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




