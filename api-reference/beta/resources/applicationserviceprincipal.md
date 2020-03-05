---
title: tipo de recurso applicationServicePrincipal
description: Uma combinação de um aplicativo e um servicePrincipalName.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9a7cc33e05c28e5552815778e86e5b1b9e7aaf06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508279"
---
# <a name="applicationserviceprincipal-resource-type"></a>tipo de recurso applicationServicePrincipal

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando uma instância de um aplicativo da Galeria de aplicativos do Azure AD é adicionada, os objetos [Application](../resources/application.md) e [UserPrincipal](../resources/serviceprincipal.md) são criados no diretório. O **applicationServicePrincipal** representa a concatenação do **aplicativo** e do objeto **servicePrincipalName** .

## <a name="methods"></a>Métodos

Nenhum

## <a name="properties"></a>Propriedades

| Propriedade | Tipo        | Descrição |
|:-------------|:------------|:------------|
|application|[application](../resources/application.md)|Representa um aplicativo registrado no Azure Active Directory.|
|servicePrincipal|[servicePrincipal](../resources/serviceprincipal.md)|Representa uma instância de um aplicativo em um diretório.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "servicePrincipal": {"@odata.type":"microsoft.graph.servicePrincipal"},
   "application": {"@odata.type":"microsoft.graph.application"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
