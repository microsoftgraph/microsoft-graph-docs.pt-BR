---
title: Tipo de recurso do azureAdJoinPolicy
description: Representa o escopo de política de um locatário Azure Active Directory que controla o registro de dispositivo usando o Azure AD Join.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a57995b3ec3228d8b7be565165667ffc39aa5338
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127898"
---
# <a name="azureadjoinpolicy-resource-type"></a>Tipo de recurso do azureAdJoinPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o escopo de política do locatário do Azure Active Directory (Azure AD) que controla a capacidade dos usuários e grupos de registrar identidades de dispositivos em sua organização usando o Azure AD Join.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedGroups|Conjunto de cadeias de caracteres|Os identificadores dos grupos que estão no escopo da política. Obrigatório quando a **propriedade appliesTo** estiver definida como `selected` . |
|allowedUsers|Conjunto de cadeias de caracteres|Os identificadores de usuários que estão no escopo da política. Obrigatório quando a **propriedade appliesTo** estiver definida como `selected` .|
|appliesTo|policyScope|Especifica se o escopo da política deve ser bloqueado ou permitir um controle fino. Os valores possíveis são: `0` (significado `none` ), `1` (significado `all` ), `2` (significado ), `selected` `3` (significado `unknownFutureValue` ). <br/><br/>O valor padrão é `1`. Quando definido como , pelo menos um identificador de grupo ou usuário deve ser especificado em `2` **allowedUsers** ou **allowedGroups**.  A configuração dessa propriedade `0` como ou remove todos os `1` identificadores em **allowedUsers** e **allowedGroups**.|
|isAdminConfigurable|Booliano|Especifica se esse escopo de política é configurável pelo administrador. O valor padrão é `false` . Quando um administrador habilitar o Intune (MEM) para gerenciar dispositivos, essa propriedade é definida como e `false` **se aplicaTo** como `1` padrão (ou `all` seja).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureAdJoinPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureAdJoinPolicy",
  "appliesTo": "String",
  "isAdminConfigurable": "Boolean",
  "allowedUsers": [
    "String"
  ],
  "allowedGroups": [
    "String"
  ]
}
```
