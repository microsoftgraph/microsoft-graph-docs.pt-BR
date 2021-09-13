---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0fa6b009fcb70208d8a4a705cb528dba3c3e2d77
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021636"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-auditing-devicemanagement-get.md)|[deviceManagement](../resources/intune-auditing-devicemanagement.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-auditing-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-auditing-devicemanagement-update.md)|[deviceManagement](../resources/intune-auditing-devicemanagement.md)|Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-auditing-devicemanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|auditEvents|Conjunto [auditEvent](../resources/intune-auditing-auditevent.md)|Eventos de auditoria|

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




