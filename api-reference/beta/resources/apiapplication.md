---
title: Tipo de recurso apiApplication
description: Especifica configurações para um aplicativo de API Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 499cc3d86ccab8706838dd3cf883b879d8bcea12
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137099"
---
# <a name="apiapplication-resource-type"></a>Tipo de recurso apiApplication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica configurações para um aplicativo que implementa uma API Web.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| Booliano | Quando verdadeiro, permite que um aplicativo use o mapeamento de declarações sem especificar uma chave de assinatura personalizada. |
|`knownClientApplications`| Coleção de GUIDs |Usado para o consentimento de ad bundling se você tiver uma solução que contenha duas partes: um aplicativo cliente e um aplicativo de API Web personalizado. Se você definir a appID do aplicativo cliente para esse valor, o usuário consente apenas uma vez com o aplicativo cliente. O Azure AD sabe que consentir com o cliente significa consentir implicitamente com a API da Web e provisionar automaticamente entidades de serviço para ambas as APIs ao mesmo tempo. O cliente e o aplicativo da API Web devem ser registrados no mesmo locatário.|
|`oauth2PermissionScopes`| coleção [permissionScope](permissionscope.md) | A definição das permissões delegadas expostas pela API Web representada por esse registro de aplicativo. Essas permissões delegadas podem ser solicitadas por um aplicativo cliente e podem ser concedidas por usuários ou administradores durante o consentimento. As permissões delegadas às vezes são conhecidas como escopos OAuth 2.0. |
|`preAuthorizedApplications`| [Coleção preAuthorizedApplication](preauthorizedapplication.md) | Lista os aplicativos cliente que são pré-autorizados com as permissões delegadas especificadas para acessar as APIs desse aplicativo. Os usuários não precisam consentir com qualquer aplicativo pré-autorizado (para as permissões especificadas). No entanto, quaisquer permissões adicionais não listadas em preAuthorizedApplications (solicitadas por meio de consentimento incremental, por exemplo) exigirão o consentimento do usuário. |
|`requestedAccessTokenVersion`| Int32 | Especifica a versão do token de acesso esperada por esse recurso. Isso altera a versão e o formato do JWT produzido independentemente do ponto de extremidade ou do cliente usado para solicitar o token de acesso. <br><br> O ponto de extremidade usado, v1.0 ou v2.0, é escolhido pelo cliente e afeta apenas a versão do id_tokens. Os recursos precisam ser explicitamente `requestedAccessTokenVersion` configuradas para indicar o formato de token de acesso com suporte. <br><br> Os valores `requestedAccessTokenVersion` possíveis para `1` são , `2` ou `null` . Se o valor for , o padrão é , que corresponde ao ponto de `null` `1` extremidade v1.0. <br><br> Se `signInAudience` no aplicativo estiver configurado como , o valor dessa propriedade deverá `AzureADandPersonalMicrosoftAccount` ser `2` |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "acceptMappedClaims": true,
  "knownClientApplications": ["Guid"],
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "requestedAccessTokenVersion": 2
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


