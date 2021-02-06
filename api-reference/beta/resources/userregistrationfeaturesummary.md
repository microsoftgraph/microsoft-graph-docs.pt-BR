---
title: Tipo de recurso userRegistrationFeatureSummary
description: Resumo de usuários capazes de autenticação multifa factor, redefinição Self-Service senha e autenticação sem senha.
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 291da483380d6e1d65b5db527128098b8b416c83
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132927"
---
# <a name="userregistrationfeaturesummary-resource-type"></a>Tipo de recurso userRegistrationFeatureSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado atual de quantos usuários em sua organização são capazes de autenticação multifafa, redefinição de senha de autoatendado e autenticação sem senha.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [usersRegisteredByFeature](../api/authenticationmethodsroot-usersregisteredbyfeature.md) | userRegistrationFeatureSummary | Obter o número de usuários capazes de autenticação multifa factor, Self-Service redefinição de senha e autenticação sem senha. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|totalUserCount|Int64|Número total de contas de usuários, excluindo aquelas bloqueadas|
|userRegistrationFeatureCounts|[Coleção userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md)|Número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha.|
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
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationFeatureCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
    }
  ]
}
```
