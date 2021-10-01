---
title: Tipo de recurso redirectUriSettings
description: Especifica o índice de um redirectUri
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 756b1e1caf92e505e62380e0ca56cc2a6f549aef
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60069343"
---
# <a name="redirecturisettings-resource-type"></a>Tipo de recurso redirectUriSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica o índice das URLs onde os tokens de usuário são enviados para entrar. Isso só é válido para aplicativos que usam SAML.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| uri | String | Especifica o URI para o que os tokens são enviados. |
|índice|Int32|Identifica o URI específico dentro da coleção redirectURIs em fluxos de SSO SAML. O padrão é `null` O índice é exclusivo em todos os redirectUris do aplicativo.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.redirectUriSettings"
}-->

``` json
{
  "@odata.type": "#microsoft.graph.redirectUriSettings",
  "uri": "String",
  "index": "Integer"
}
```
