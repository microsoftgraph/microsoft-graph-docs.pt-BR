---
title: tipo de recurso de onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 30ff6908a42a690e07d71b5d0c62fcb22dea3c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842536"
---
# <a name="onpremisespublishing-resource-type"></a>tipo de recurso de onPremisesPublishing

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customDomainCertificate|Cadeia de caracteres|Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso. Nulo ao usar o domínio padrão.|
|externalAuthenticationType|Cadeia de caracteres|Detalha a configuração de pré-autenticação para os aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.|
|externalUrl|Cadeia de caracteres|A url externa publicada para o aplicativo. Por exemplohttps://intranet-contoso.msappproxy.net/  |
|internalUrl|Cadeia de caracteres|A url interna do aplicativo. Por exemplohttps://intranet/ |
|isOnPremPublishingEnabled|Booliano|Indica se o aplicativo atualmente está sendo publicado ou não.|
|applicationServerTimeout|Cadeia de caracteres|A duração o conector aguardará uma resposta do aplicativo back-end antes de fechar a conexão. Os valores possíveis são `default`, `long`. Uso `long` se seu servidor demorar mais de 75-60 segundos para responder às solicitações. Além disso, experimente `long` se não for possível acessar o aplicativo e o status de erro é "Backend Timeout".|
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
