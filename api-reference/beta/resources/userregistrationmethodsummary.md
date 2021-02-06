---
title: Tipo de recurso userRegistrationMethodSummary
description: Resumo do número de usuários registrados para cada método de autenticação.
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6ff9a079ddce0df5031eef2b1374ebb1d233d56d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132913"
---
# <a name="userregistrationmethodsummary-resource-type"></a>Tipo de recurso userRegistrationMethodSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Resumo do número de usuários registrados para cada método de autenticação.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [usersRegisteredByMethod](../api/authenticationmethodsroot-usersregisteredbymethod.md) | userRegistrationMethodSummary | Obter o número de usuários registrados para cada método de autenticação. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|totalUserCount|Int64|Número total de usuários no locatário.|
|userRegistrationMethodCounts|[Coleção userRegistrationMethodCount](../resources/userregistrationmethodcount.md)|Número de usuários registrados para cada método de autenticação.|
|userRoles|includedUserRoles|Tipo de função de usuário. Os valores possíveis são: `all`, `privilegedAdmin`, `admin`, `user`.|
|userTypes|includedUserTypes|Tipo de usuário. Os valores possíveis são: `all`, `member`, `guest`.|

O valor `privilegedAdmin` consiste nas seguintes funções de administrador privilegiado:

* Administrador global
* Administrador de segurança
* Administrador de acesso condicional
* Administrador do Exchange
* Administrador do SharePoint
* Administrador de help desk
* Administrador de faturamento
* Administrador de usuários
* Administrador de autenticação

O valor inclui todas as funções de administrador do `admin` Azure AD. 

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationMethodCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationMethodCount"
    }
  ]
}
```
