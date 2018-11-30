---
title: tipo de recurso de onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 8dba505347fc12d3c4a8521ebe32551d738dc4a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037022"
---
# <a name="onpremisespublishing-resource-type"></a>tipo de recurso de onPremisesPublishing

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customDomainCertificate|String|Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso. Nulo ao usar o domínio padrão.|
|externalAuthenticationType|String|Detalha a configuração de pré-autenticação para os aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.|
|externalUrl|String|A url externa publicada para o aplicativo. Por exemplohttps://intranet-contoso.msappproxy.net/  |
|internalUrl|String|A url interna do aplicativo. Por exemplohttps://intranet/ |
|isOnPremPublishingEnabled|Booliano|Indica se o aplicativo atualmente está sendo publicado ou não.|
|applicationServerTimeout|String|A duração o conector aguardará uma resposta do aplicativo back-end antes de fechar a conexão. Os valores possíveis são `default`, `long`. Uso `long` se seu servidor demorar mais de 75-60 segundos para responder às solicitações. Além disso, experimente `long` se não for possível acessar o aplicativo e o status de erro é "Backend Timeout".|
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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
