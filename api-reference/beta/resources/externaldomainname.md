---
title: Tipo de recurso externalDomainName
description: Nome de domínio da organização externa um locatário Azure Active Directory (Azure AD) atuando como o locatário de recursos está tentando configurar a federação com.
author: namkedia
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a84c13d4800d79263ef63423ef390846eecb5ec2
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696992"
---
# <a name="externaldomainname-resource-type"></a>Tipo de recurso externalDomainName

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o nome de domínio da organização externa em que um locatário do Azure Active Directory (Azure AD) atuando como o locatário de recursos está tentando configurar a federação.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Nome de domínio da organização externa com a que o locatário do Azure AD está federando. Herdado da [entidade](../resources/entity.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalDomainName",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalDomainName",
  "id": "String (identifier)"
}
```
