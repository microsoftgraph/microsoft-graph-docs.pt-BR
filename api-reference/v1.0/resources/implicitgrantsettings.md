---
title: Tipo de recurso implicitGrantSettings
description: Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito OAuth 2.0. Propriedades separadas estão disponíveis para solicitar ID e acessar tokens como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das seguintes propriedades deve ser definida como true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: bfe1e38dfdbdeffb81d34db0f68628c58a37421ee6da260be08e4c6f05c37015
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155131"
---
# <a name="implicitgrantsettings-resource-type"></a>Tipo de recurso implicitGrantSettings

Namespace: microsoft.graph

Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito OAuth 2.0. Propriedades separadas estão disponíveis para solicitar ID e acessar tokens como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das seguintes propriedades deve ser definida como true.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Booliano | Especifica se esse aplicativo Web pode solicitar um token de ID usando o fluxo implícito OAuth 2.0.|
|enableAccessTokenIssuance| Booliano | Especifica se esse aplicativo Web pode solicitar um token de acesso usando o fluxo implícito OAuth 2.0.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```

