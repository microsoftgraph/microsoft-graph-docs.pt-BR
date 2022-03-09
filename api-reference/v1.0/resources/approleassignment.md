---
title: Tipo de recurso appRoleAssignment
description: Usado para registrar quando um usuário, grupo ou entidade de serviço é atribuído a uma função de aplicativo na entidade de serviço de um aplicativo. Você pode criar, ler e excluir atribuições de função de aplicativo.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 67e3684b9b0668ae7adce632dd754eb813bf1162
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333194"
---
# <a name="approleassignment-resource-type"></a>Tipo de recurso appRoleAssignment

Namespace: microsoft.graph

Utilizado para registro quando um usuário, grupo ou entidade de serviço recebe uma função de aplicativo para um aplicativo.

Uma atribuição de função de aplicativo é uma relação entre a entidade de segurança atribuída (um usuário, um grupo ou uma entidade de serviço), um aplicativo de recursos (a entidade de serviço do aplicativo) e uma função de aplicativo definida no aplicativo de recurso.

Quando a [função do aplicativo](approle.md) que foi atribuída a um principal tem uma propriedade de **valor** não vazio, isso será incluído na declaração de **funções** de tokens onde o sujeito é o principal atribuído (por exemplo, respostas SAML, tokens de ID, tokens de acesso que identificam um sinal no usuário ou um token de acesso que identifica um principal de serviço). Aplicativos e APIs usam essas declarações como parte de sua lógica de autorização.

É possível atribuir uma função de aplicativo diretamente a um usuário. Se uma função de aplicativo for atribuída a um grupo, os membros diretos do grupo também serão considerados atribuídos à função de aplicativo. Quando um usuário recebe uma função de aplicativo para um aplicativo, o bloco do aplicativo é exibido no portal [MyApps](/azure/active-directory/user-help/my-apps-portal-end-user-access) e no[inicializador de aplicativos do Microsoft 365](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).

Quando um usuário ou administrador consentir a uma [permissão somente para aplicativo](/azure/active-directory/develop/v2-permissions-and-consent#permission-types), será criada uma atribuição de função de aplicativo onde a entidade de segurança atribuída é a entidade de serviço do aplicativo cliente e o recurso é a entidade de serviço da API de destino.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| appRoleId | Guid | O identificador (**id**) da [função do aplicativo](approle.md) que está atribuída à entidade de segurança. Essa função de aplicativo deve ser exposta na propriedade **appRoles** na entidade de serviço do aplicativo de recurso (**ResourceId**). Se o aplicativo de recurso não tiver declarado todas as funções do aplicativo, uma ID de função de aplicativo padrão de `00000000-0000-0000-0000-000000000000` poderá ser especificada para sinalizar que a entidade de segurança está atribuída ao aplicativo de recursos sem nenhuma função específica do aplicativo. Obrigatório durante a criação.  |
| createdDateTime | DateTimeOffset | A hora em que a atribuição de função do aplicativo foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre na hora UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.  |
| id | Cadeia de caracteres | Um identificador exclusivo para a chave **appRoleAssignment**. Não pode ser anulado. Somente leitura. |
| principalDisplayName | Cadeia de caracteres |O nome de exibição do usuário, grupo ou entidade de serviço que recebeu a atribuição de função de aplicativo. Somente leitura. Suporta `$filter` (`eq` e `startswith`). |
| principalId | Guid | O identificador exclusivo (**id**) para o [usuário](user.md), [grupo](group.md), ou [entidade de serviço](serviceprincipal.md) sendo concedido a função do aplicativo. Necessário na criação.  |
| principalType | Cadeia de caracteres | O tipo da entidade de segurança atribuída. Isso pode ser `User`, `Group`ou `ServicePrincipal`. Somente leitura.  |
| resourceDisplayName | Cadeia de caracteres | O nome de exibição da entidade de serviço da função do aplicativo para o qual a atribuição foi feita.  |
| resourceId | Guid |O identificador exclusivo (**id**) do [principal de serviço](serviceprincipal.md) de recurso para o qual a atribuição é feita. Obrigatório na criação. Suporta `$filter` (`eq` apenas). |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "appRoleId": "Guid",
  "createdDateTime": "String (timestamp)",
  "id": "String",
  "principalDisplayName": "String",
  "principalId": "Guid",
  "principalType": "String",
  "resourceDisplayName": "String",
  "resourceId": "Guid"
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
