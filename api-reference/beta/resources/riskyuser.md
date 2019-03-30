---
title: tipo de recurso riskyUsers
description: Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3265ea40903ca2c5c10272f5df280bd3715af366
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003717"
---
# <a name="riskyusers-resource-type"></a>tipo de recurso riskyUsers

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).

>**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar riskyUsers](../api/riskyusers-list.md) | [riskyUsers](riskyUser.md) |Listar usuários arriscados e suas propriedades.|
|[Obter riskyUsers](../api/riskyusers-get.md) | [riskyUsers](riskyUser.md)|Obtenha um usuário arriscado específico e suas propriedades.|
|[Confirmar riskyUsers comprometido](../api/riskyusers-confirmcompromised.md)|Confirmar um usuário arriscado como comprometido.|
|[Ignorar riskyUsers](../api/riskyusers-dismiss.md)|DesCartar o risco de um usuário arriscado.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|`id`|`string`|ID exclusiva do usuário em risco|
|`isDeleted`|`bool`|Indica se o usuário é excluído. Os valores possíveis são `true`:,`false`|
|`isGuest`|`bool`|Indica se o usuário é um usuário convidado. Os valores possíveis são: `true` e `false`. True se a identidade do usuário está fora do locatário em consideração. Este usuário pode ser um usuário B2B ou B2C com identidade no Azure AD, no MSA ou no provedor de identidade de terceiros. False se a identidade do usuário está dentro do locatário em consideração|
|`isProcessing`|`bool`|Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend|
|`risk`|[risco](risk.md)|Estado de usuário arriscado|
|`riskLastUpdatedDateTime`|`datetime`|A data e a hora em que o usuário arriscado foi atualizado pela última vez|
|`userDisplayName`|`string`|Nome de exibição do usuário arriscado|
|`userPrincipalName`|`string`|Nome UPN de usuário arriscado|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
 "id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isProcessing": "boolean",
"isDeleted": "boolean",
"risk": {"@odata.type": "microsoft.graph.risk"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
