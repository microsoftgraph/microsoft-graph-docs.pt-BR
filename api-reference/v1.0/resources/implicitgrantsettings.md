---
title: Tipo de recurso implicitGrantSettings
description: Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2.0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 58509ff0f0264a683aaae9c83d60e0f041ef0af7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133277"
---
# <a name="implicitgrantsettings-resource-type"></a>Tipo de recurso implicitGrantSettings

Namespace: microsoft.graph

Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2.0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Booliano | Especifica se esse aplicativo Web pode solicitar um token de ID usando o fluxo implícito do OAuth 2.0.|
|enableAccessTokenIssuance| Booliano | Especifica se esse aplicativo Web pode solicitar um token de acesso usando o fluxo implícito do OAuth 2.0.|

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

