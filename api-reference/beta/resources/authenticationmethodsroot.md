---
title: tipo de recurso authenticationMethodsRoot
description: Contêiner para propriedades de navegação para recursos de autenticação do Azure AD.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e01fe33d73d67058bf765d3562c77ea657630ea6
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2021
ms.locfileid: "61403196"
---
# <a name="authenticationmethodsroot-resource-type"></a>tipo de recurso authenticationMethodsRoot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner para propriedades de navegação para recursos de autenticação do Azure AD.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String| Um identificador exclusivo. Herdado da [entidade](../resources/entity.md).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRoot",
  "id": "String (identifier)"
}
```