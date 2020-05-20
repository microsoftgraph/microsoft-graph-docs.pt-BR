---
title: tipo de recurso apiApplication
description: Especifica as configurações para um aplicativo da API Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 2b5676b9a6dce715121b6d5a711cab0e83f948f6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290585"
---
# <a name="apiapplication-resource-type"></a>tipo de recurso apiApplication

Namespace: microsoft.graph

Especifica configurações para um aplicativo que implementa uma API Web.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| Booliano | Quando true, permite que um aplicativo use o mapeamento de declarações sem especificar uma chave de assinatura personalizada. |
|`knownClientApplications`| Coleção de GUIDs |Usado para o consentimento de agrupamento se você tiver uma solução que contenha duas partes: um aplicativo cliente e um aplicativo de API Web personalizado. Se você definir a appID do aplicativo cliente com esse valor, o usuário só consenti uma vez para o aplicativo cliente. O Azure AD sabe que a reenvio para o cliente significa implicitamente Confira a API Web e automaticamente provisiona entidades de serviço para ambas as APIs ao mesmo tempo. O cliente e o aplicativo da API Web devem ser registrados no mesmo locatário.|
|`oauth2PermissionScopes`| coleção [permissionScope](permissionscope.md) | A definição das permissões delegadas expostas pela API Web representada por este registro de aplicativo. Essas permissões delegadas podem ser solicitadas por um aplicativo cliente e podem ser concedidas por usuários ou administradores durante o consentimento. As permissões delegadas às vezes são chamadas de escopos OAuth 2,0. |
|`preAuthorizedApplications`| coleção [preauthorizedapplication e](preauthorizedapplication.md) | Lista os aplicativos cliente que são previamente autorizados com as permissões delegadas especificadas para acessar as APIs desse aplicativo. Os usuários não precisam ser consentidos em qualquer aplicativo pré autorizado (para as permissões especificadas). No entanto, qualquer permissão adicional que não esteja listada no preAuthorizedApplications (solicitado por meio de consentimento incremental, por exemplo) exigirá o consentimento do usuário. |
|`requestedAccessTokenVersion`| Int32 | Especifica a versão do token de acesso esperada por este recurso. Isso altera a versão e o formato do JWT produzido independentemente do ponto de extremidade ou cliente usado para solicitar o token de acesso. <br><br> O ponto de extremidade usado, v 1.0 ou v 2.0, é escolhido pelo cliente e só impacta a versão do id_tokens. Os recursos precisam ser configurados explicitamente `requestedAccessTokenVersion` para indicar o formato do token de acesso suportado. <br><br> Os valores possíveis para `requestedAccessTokenVersion` são `1` , `2` , ou `null` . Se o valor for `null` , este padrão será `1` , que corresponde ao ponto de extremidade v 1.0. <br><br> Se `signInAudience` no aplicativo estiver configurado como `AzureADandPersonalMicrosoftAccount` , o valor dessa propriedade deverá ser`2` |

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
