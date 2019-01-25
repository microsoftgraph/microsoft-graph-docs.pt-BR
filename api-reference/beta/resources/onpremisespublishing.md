---
title: tipo de recurso de onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508178"
---
# <a name="onpremisespublishing-resource-type"></a>tipo de recurso de onPremisesPublishing

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customDomainCertificate|String|Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso. Nulo ao usar o domínio padrão.|
|externalAuthenticationType|String|Detalha a configuração de pré-autenticação para os aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.|
|externalUrl|String|A url externa publicada para o aplicativo. Por exemplo:  |
|internalUrl|String|A url interna do aplicativo. Por exemplo: |
|isOnPremPublishingEnabled|Booliano|Indica se o aplicativo atualmente está sendo publicado ou não.|
|applicationServerTimeout|String|A duração o conector aguardará uma resposta do aplicativo back-end antes de fechar a conexão. Os valores possíveis são: `default` e `long`. Uso `long` se seu servidor demorar mais de 75-60 segundos para responder às solicitações. Além disso, experimente `long` se não for possível acessar o aplicativo e o status de erro é "Backend Timeout".|
|isTranslateHostHeaderEnabled|Booliano|Indica se o aplicativo deve traduzir urls em cabeçalhos de resposta. Isso inclui a definição de site correto para os cookies.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
