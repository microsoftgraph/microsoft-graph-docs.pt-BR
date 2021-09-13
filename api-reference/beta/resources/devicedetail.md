---
title: Tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar.
ms.localizationpriority: medium
author: spunukol
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a53c22d62462b02325594722d7be9ba4fc5a671c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101972"
---
# <a name="devicedetail-resource-type"></a>Tipo de recurso deviceDetail

Namespace: microsoft.graph Indica detalhes do dispositivo associados a um dispositivo usado para entrar. Inclui informações como navegador de dispositivos e informações do sistema operacional, se o dispositivo for gerenciado pelo Azure AD.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Navegador|Cadeia de Caracteres|Indica as informações do navegador do usado para entrar.|
|deviceId|Cadeia de caracteres|Refere-se à UniqueID do dispositivo usado para entrar.|
|displayName|Cadeia de caracteres|Refere-se ao nome do dispositivo usado para entrar.|
|isCompliant|Booliano|Indica se o dispositivo está em conformidade ou não.|
|isManaged|Booliano|Indica se o dispositivo é gerenciado ou não.|
|operatingSystem|String|Indica o nome e a versão do sistema operacional usados para entrar.|
|trustType|String|Indica informações sobre se o dispositivo conectado é Workplace Joined, AzureAD Joined, Domain Joined. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


