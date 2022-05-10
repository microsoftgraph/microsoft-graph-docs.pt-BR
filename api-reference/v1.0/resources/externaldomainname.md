---
title: Tipo de recurso externalDomainName
description: Nome de domínio da organização externa com a qual um Azure Active Directory (Azure AD) atuando como o locatário do recurso está federando.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: de723382ddfdbb7ef68c871e84498560d2b03ce8
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296557"
---
# <a name="externaldomainname-resource-type"></a>Tipo de recurso externalDomainName

Namespace: microsoft.graph

Representa o nome de domínio da organização externa com a qual um locatário Azure Active Directory (Azure AD) atuando como o locatário do recurso está federando.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Nome de domínio da organização externa com a qual Azure AD locatário está federando. Herdado da [entidade](../resources/entity.md).|

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
