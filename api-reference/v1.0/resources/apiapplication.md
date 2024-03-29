---
title: Tipo de recurso apiApplication
description: Especifica configurações para um aplicativo de API Web.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 9cde2098a4ac7a1c9cd8d143513e0b6294a08cd0
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854689"
---
# <a name="apiapplication-resource-type"></a>Tipo de recurso apiApplication

Namespace: microsoft.graph

Especifica configurações para um aplicativo que implementa uma API Web.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|acceptMappedClaims| Booliano | Quando `true`, permite que um aplicativo use o mapeamento de declarações sem especificar uma chave de assinatura personalizada. |
|knownClientApplications| Coleção GUID |Usado para o consentimento em comum se você tiver uma solução que contenha duas partes: um aplicativo cliente e um aplicativo de API Web personalizado. Se você definir a appID do aplicativo cliente para esse valor, o usuário só consente uma vez no aplicativo cliente. O Azure AD sabe que consentir com o cliente significa consentir implicitamente a API da Web e provisionar automaticamente as entidades de serviço para ambas as APIs ao mesmo tempo. Tanto o cliente quanto o aplicativo api web devem ser registrados no mesmo locatário.|
|oauth2PermissionScopes| coleção [permissionScope](permissionscope.md) | A definição das permissões delegadas expostas pela API web representada pelo registro desse aplicativo. Essas permissões delegadas podem ser solicitadas por um aplicativo cliente e podem ser concedidas por usuários ou administradores durante o consentimento. As permissões delegadas às vezes são conhecidas como escopos OAuth 2.0. |
|preAuthorizedApplications| [coleção preAuthorizedApplication](preauthorizedapplication.md) | Lista os aplicativos cliente pré-autorizados com as permissões delegadas especificadas para acessar as APIs desse aplicativo. Os usuários não precisam consentir com nenhum aplicativo pré-autorizado (para as permissões especificadas). No entanto, quaisquer permissões adicionais não listadas em preAuthorizedApplications (solicitadas por meio do consentimento incremental, por exemplo) exigirão o consentimento do usuário. |
|requestedAccessTokenVersion| Int32 | Especifica a versão do token de acesso esperada por esse recurso. Isso altera a versão e o formato do JWT produzido independentemente do ponto de extremidade ou cliente usado para solicitar o token de acesso. <br><br> O ponto de extremidade usado, v1.0 ou v2.0, é escolhido pelo cliente e afeta apenas a versão do id_tokens. Os recursos precisam configurar explicitamente **requestedAccessTokenVersion** para indicar o formato de token de acesso suportado. <br><br> Os valores possíveis **para requestedAccessTokenVersion** são `1`, `2`ou `null`. Se o valor for `null`, isso padrão será `1`, que corresponde ao ponto de extremidade v1.0. <br><br> Se **signInAudience** no aplicativo estiver configurado como `AzureADandPersonalMicrosoftAccount`, o valor dessa propriedade deve ser `2` |

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
  "knownClientApplications": ["GUID"],
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

