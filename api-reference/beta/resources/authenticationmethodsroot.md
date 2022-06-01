---
title: Tipo de recurso authenticationMethodsRoot
description: Contêiner para propriedades de navegação para Azure AD de métodos de autenticação.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: cc86e2ff67f7c628406aa90aca5bd00d03101272
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820480"
---
# <a name="authenticationmethodsroot-resource-type"></a>Tipo de recurso authenticationMethodsRoot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner para propriedades de navegação para Azure AD de métodos de autenticação.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres| Um identificador exclusivo. Herdado da [entidade](../resources/entity.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|userRegistrationDetails|[userRegistrationDetails](../resources/userRegistrationDetails.md)| Representa o estado dos métodos de autenticação de um usuário, incluindo quais métodos são registrados e quais recursos o usuário é registrado e capaz (como autenticação multifator, redefinição de senha de autoatendimento e autenticação sem senha).|

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