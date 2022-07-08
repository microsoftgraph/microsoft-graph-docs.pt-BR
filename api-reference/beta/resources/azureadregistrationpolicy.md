---
title: Tipo de recurso azureADRegistrationPolicy
description: Representa o escopo da política de um locatário do Azure Active Directory que controla o registro do dispositivo usando Azure AD registrado.
author: myra-ramdenbourg
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 95c715578dc6944b0d678314b1bb9604f1b0b985
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690075"
---
# <a name="azureadregistrationpolicy-resource-type"></a>Tipo de recurso azureADRegistrationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o escopo da política do locatário do Azure Active Directory (Azure AD) que controla a capacidade de usuários e grupos registrarem identidades de dispositivo em sua organização usando Azure AD **registrados**. Para obter mais informações, consulte [O que é uma identidade do dispositivo?](/azure/active-directory/devices/overview).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedGroups|String collection| Os identificadores dos grupos que estão no escopo da política. Essa propriedade ou **allowedUsers** é necessária quando a **propriedade appliesTo** é definida como `selected`. |
|allowedUsers|Coleção de cadeias de caracteres| Os identificadores de usuários que estão no escopo da política. Essa propriedade ou **allowedGroups** é necessária quando a **propriedade appliesTo** é definida como `selected`. |
|Appliesto|policyScope|Especifica se é necessário bloquear ou permitir um controle refinado do escopo da política. Os valores possíveis são: `0` (significado `none`), `1` (significado `all`), `2` (significado `selected`), `3` (significado `unknownFutureValue`). <br/><br/>O valor padrão é `1`. Quando definido como `2`, pelo menos um identificador de usuário ou grupo deve ser especificado em **allowedUsers** ou **allowedGroups**.  Definir essa propriedade como `0` ou remover `1` todos os identificadores em **allowedUsers** e **allowedGroups**.|
|isAdminConfigurable|Booleano|Especifica se esse escopo de política é configurável pelo administrador. O valor padrão é `false`. Quando um administrador habilitou Intune (MEM) para gerenciar **dispositivos** `1` , `false` essa propriedade é definida como e aplica os padrões a (significando `all`). |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureADRegistrationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureADRegistrationPolicy",
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
