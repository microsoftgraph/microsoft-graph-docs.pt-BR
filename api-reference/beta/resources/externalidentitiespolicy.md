---
title: Tipo de recurso externalIdentitiesPolicy
description: Representa a política de todo o locatário que controla se os usuários externos podem deixar um locatário Azure AD por meio de controles de autoatendimento.
author: KuiGithui
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 49701027e0dace54a8f74a2eebef0115329de9a4
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768333"
---
# <a name="externalidentitiespolicy-resource-type"></a>Tipo de recurso externalIdentitiesPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a política de todo o locatário que controla se os usuários externos podem deixar o locatário Azure AD convidado por meio de controles de autoatendimento. Quando permitido pelo administrador, os usuários externos podem deixar o locatário Azure AD convidado por meio **do menu de** organizações do portal [Minha Conta](https://myaccount.microsoft.com/).

Herda de [policyBase](../resources/policybase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter externalIdentitiesPolicy](../api/externalidentitiespolicy-get.md)|[externalIdentitiesPolicy](../resources/externalidentitiespolicy.md)|Leia as propriedades e as relações de um [objeto externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) .|
|[Atualizar externalIdentitiesPolicy](../api/externalidentitiespolicy-update.md)|[externalIdentitiesPolicy](../resources/externalidentitiespolicy.md)|Atualize as propriedades de um [objeto externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowDeletedIdentitiesDataRemoval|Booliano|Notifica Azure AD se deve limpar as informações do usuário sobre a identidade externa, do locatário convidado, quando o usuário é excluído em seu locatário inicial. |
|allowExternalIdentitiesToLeave|Booliano|Define se os usuários externos podem sair do locatário convidado. Se definido como `false`, os controles de autoatendimento não serão habilitados e o administrador do locatário convidado deverá remover manualmente o usuário externo do locatário convidado.|
|displayName|String|O nome da política. Herdado do [policyBase](../resources/policybase.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalIdentitiesPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalIdentitiesPolicy",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "allowExternalIdentitiesToLeave": "Boolean",
  "allowDeletedIdentitiesDataRemoval": "Boolean"
}
```

