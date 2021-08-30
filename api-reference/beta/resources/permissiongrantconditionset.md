---
title: tipo de recurso permissionGrantConditionSet
description: Especifica uma regra de correspondência com condições em que um evento é incluído ou excluído de uma política de concessão de permissão.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 8e13beea466e1a6d4d950fcfc81c0546d0a62e57
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58694644"
---
# <a name="permissiongrantconditionset-resource-type"></a>tipo de recurso permissionGrantConditionSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um conjunto de condições de concessão de permissão é usado para especificar uma regra de correspondência em uma [política de concessão de permissão](permissiongrantpolicy.md) para incluir ou excluir um evento de concessão de permissão.

Um conjunto de condições para concessão de permissão contém várias condições. Para que um evento corresponda a um conjunto de condições de concessão de permissão, todas as condições devem ser atendidas.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo |Descrição|
|:---------------|:--------|:----------|
| id | String | O identificador exclusivo para o conjunto de condições de concessão de permissão. Chave. Somente leitura. |
| permissionClassification | String | O [classificação de permissão](delegatedpermissionclassification.md)pela permissão sendo concedida, ou `all` para corresponder a qualquer classificação de permissão (incluindo permissões que não são classificadas). O padrão é `all`. |
| permissionType | permissionType | O tipo de permissão da permissão sendo concedida. Valores possíveis: `application` para permissões de aplicativos (por exemplo, funções de aplicativos) ou`delegated` para permissões delegadas. O valor `delegatedUserConsentable` indica que as permissões delegadas que não foram configuradas pelo fornecedor da API exigem o consentimento do administrador — esse valor pode ser usado em políticas de concessão de permissão interna, mas não pode ser usado em políticas de concessão de permissão personalizadas. Obrigatório. |
| resourceApplication | String | O **appId** do aplicativo de recursos (por exemplo, a API) para o qual uma permissão está sendo concedida ou `any` para corresponder a qualquer aplicativo de recurso ou API. O padrão é `any`. |
| permissões | Conjunto de cadeia de caracteres | A lista de **identificação** valores para as permissões específicas corresponderem ou uma lista com o valor único `all` para combinar com qualquer permissão. A **identificação** de permissões delegadas podem ser encontradas na propriedade **publishedPermissionScopes** do objeto [**servicePrincipal**](serviceprincipal.md) da API. A **identificação** das permissões do aplicativo podem ser encontradas na propriedade **appRoles** do objeto [**servicePrincipal**](serviceprincipal.md) da API. A **identificação** de permissões de aplicativos específicas do recurso pode ser encontrada na propriedade **resourceSpecificApplicationPermissions** do objeto [**servicePrncipal**](serviceprincipal.md) da API. O padrão é o valor único `all`. |
| clientApplicationIds | Coleção de cadeias de caracteres | A lista de **appld** valores para os aplicativos cliente corresponderem ou uma lista com o valor único `all` para corresponder a qualquer aplicativo cliente. O padrão é o valor único `all`. |
| clientApplicationTenantIds | Coleção de cadeias de caracteres | Uma lista de IDs de locatário do Azure Active Directory em que o aplicativo cliente está registrado ou uma lista com o valor único `all` para corresponder aos aplicativos clientes registrados em qualquer locatário. O padrão é o valor único `all`. |
| clientApplicationPublisherIds | Coleção de cadeias de caracteres | Uma lista de IDs do Microsoft Partner Network (MPN) para editores verificados do aplicativo cliente ou uma lista com o valor único `all` para combinar com aplicativos cliente de qualquer editor. O padrão é o valor único `all`. |
| clientApplicationsFromVerifiedPublisherOnly | Booleano | Configure para `true` para corresponder apenas a aplicativos cliente com um fornecedor verificado. Configure para `false` para corresponder a qualquer aplicativo cliente, mesmo que não tenha um fornecedor verificado. O padrão é `false`. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
}-->

```json
{
    "id": "string (identifier)",
    "permissionClassification": "string",
    "permissionType": "string",
    "resourceApplication": "string",
    "permissions": [ "string" ],
    "clientApplicationIds": [ "string" ],
    "clientApplicationTenantIds": [ "string" ],
    "clientApplicationPublisherIds": [ "string" ],
    "clientApplicationsFromVerifiedPublisherOnly": false
}
```
