---
title: Tipo de recurso plannerAssignment
description: Usado para gravar quando um usuário, grupo ou entidade de serviço é atribuído a uma função de aplicativo na entidade de serviço de um aplicativo. Você pode criar, ler e excluir atribuições de função de aplicativo.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ae7c770d97640f6af63dcb594b7f624fb119f1e6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896788"
---
# <a name="approleassignment-resource-type"></a>Tipo de recurso plannerAssignment

Namespace: microsoft.graph

Usado para gravar quando um usuário, grupo ou entidade de serviço recebe uma função de aplicativo para um aplicativo.

Uma atribuição de função de aplicativo é uma relação entre a entidade de segurança atribuída (um usuário, um grupo ou uma entidade de serviço), um aplicativo de recurso (a entidade de serviço do aplicativo) e uma função de aplicativo definida no aplicativo de recurso.

Quando a [função de aplicativo](approle.md) que foi atribuída a uma entidade de segurança tem uma propriedade de **valor** não vazio, ela será incluída na declaração de **funções** de tokens em que o assunto é a entidade de segurança atribuída (por exemplo, respostas SAML, tokens de ID, tokens de acesso que identificam um usuário conectado ou um token de acesso que identifica uma entidade de serviço). Aplicativos e APIs usam essas declarações como parte de sua lógica de autorização.

Um usuário pode ser atribuído diretamente a uma função de aplicativo. Se uma função de aplicativo for atribuída a um grupo, os membros diretos do grupo também serão considerados como a função de aplicativo atribuída. Quando um usuário recebe uma função de aplicativo para um aplicativo, um bloco para esse aplicativo é exibido no [portal myapps](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access) do usuário e no [inicializador de aplicativos do Microsoft 365](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).

Uma atribuição de função de aplicativo onde a entidade atribuída é uma entidade de serviço é uma concessão [de permissão somente de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types) . Quando um usuário ou administrador se envia a uma permissão somente de aplicativo, uma atribuição de função de aplicativo é criada onde a entidade de segurança atribuída é a entidade de serviço para o aplicativo cliente e o recurso é a entidade de serviço da API de destino.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Um identificador exclusivo para a chave **appRoleAssignment** . Não anulável. Somente leitura. |
| creationTimestamp | DateTimeOffset | A hora em que a atribuição de função de aplicativo foi criada. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. Não oferece suporte `$filter` . |
| principalId | Guid | O identificador exclusivo (**ID**) do [usuário](user.md), [grupo](group.md) ou [entidade de serviço](serviceprincipal.md) que recebeu a função de aplicativo. Obrigatório ao criar. Não oferece suporte `$filter` . |
| principalType | String | O tipo da entidade de segurança atribuída. Pode ser “User”, “Group” ou “ServicePrincipal”. Somente leitura. Não oferece suporte `$filter` . |
| principalDisplayName | String |O nome de exibição do usuário, grupo ou entidade de serviço que recebeu a atribuição da função de aplicativo. Somente leitura. Suporta `$filter` ( `eq` e `startswith` ). |
| resourceId | Guid |O identificador exclusivo (**ID**) da entidade de [serviço](serviceprincipal.md) de recurso para a qual a atribuição foi feita. Obrigatório ao criar. Suporta `$filter` ( `eq` somente). |
| resourceDisplayName | String | O nome de exibição da entidade de serviço do aplicativo de recurso para a qual a atribuição foi feita. Não oferece suporte `$filter` . |
| appRoleId | Guid | O identificador (**ID**) da [função de aplicativo](approle.md) que é atribuída à entidade de segurança. Essa função de aplicativo deve ser exposta na propriedade **appRoles** na entidade de serviço do aplicativo de recurso (**ResourceId**). Se o aplicativo de recursos não tiver declarado nenhuma função de aplicativo, uma ID de função de aplicativo padrão `00000000-0000-0000-0000-000000000000` pode ser especificada para sinalizar que a entidade de segurança é atribuída ao aplicativo de recursos sem nenhuma função de aplicativo específica. Obrigatório ao criar. Não oferece suporte `$filter` . |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "id": "string",
  "creationTimestamp": "String (timestamp)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid",
  "appRoleId": "guid"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
