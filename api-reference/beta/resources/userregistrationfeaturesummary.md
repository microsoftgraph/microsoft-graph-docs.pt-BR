---
title: Tipo de recurso userRegistrationFeatureSummary
description: Resumo de usuários com capacidade para Autenticação Multifator, Self-Service redefinição de senha e autenticação sem senha.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b058276eaa3bc9f12dbe46ddc33afbe06b0bc2f2
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820144"
---
# <a name="userregistrationfeaturesummary-resource-type"></a>Tipo de recurso userRegistrationFeatureSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado atual de quantos usuários em sua organização são capazes de autenticação multifator, redefinição de senha de autoatendimento e autenticação sem senha.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [usersRegisteredByFeature](../api/authenticationmethodsroot-usersregisteredbyfeature.md) | userRegistrationFeatureSummary | Obtenha o número de usuários capazes de autenticação multifator, redefinição Self-Service senha e autenticação sem senha. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|totalUserCount|Int64|Número total de contas de usuários, excluindo aquelas que estão bloqueadas|
|userRegistrationFeatureCounts|[coleção userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md)|Número de usuários registrados ou capazes de autenticação multifator, Self-Service redefinição de senha e autenticação sem senha.|
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

O valor `admin` inclui todas as Azure AD de administrador. 

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
