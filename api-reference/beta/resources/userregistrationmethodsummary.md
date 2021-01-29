---
title: Tipo de recurso userRegistrationMethodSummary
description: Resumo do número de usuários registrados para cada método de autenticação.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 4f4d391291008bcbca1d017360bcb8caf3aea067
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052557"
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