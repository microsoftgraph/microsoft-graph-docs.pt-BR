---
title: tipo de recurso authenticationMethodsRoot
description: Contêiner para propriedades de navegação para recursos de autenticação do Azure AD.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: def78eddd43cdb7ea738d32e25c8d90adb23fbc4
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201684"
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
|id|Cadeia de caracteres| Um identificador exclusivo. Herdado da [entidade](../resources/entity.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|userRegistrationDetails|[userRegistrationDetails](../resources/userRegistrationDetails.md)| Representa o estado dos métodos de autenticação de um usuário, incluindo quais métodos são registrados e quais recursos o usuário é registrado e capaz (como autenticação multifato, redefinição de senha de autoatendados e autenticação sem senha).|

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