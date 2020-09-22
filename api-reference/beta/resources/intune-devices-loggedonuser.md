---
title: tipo de recurso loggedOnUser
description: Usuário conectado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f953c176bf6163df0a53fc4996a29de060ebe191
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081276"
---
# <a name="loggedonuser-resource-type"></a>tipo de recurso loggedOnUser

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Usuário conectado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userId|Cadeia de caracteres|ID de usuário|
|lastLogOnDateTime|DateTimeOffset|Data e hora em que o usuário faz logon|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```






