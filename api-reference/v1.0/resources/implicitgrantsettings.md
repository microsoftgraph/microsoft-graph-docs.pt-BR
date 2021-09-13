---
title: Tipo de recurso implicitGrantSettings
description: Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito OAuth 2.0. Propriedades separadas estão disponíveis para solicitar ID e acessar tokens como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das seguintes propriedades deve ser definida como true.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 2ccf78ded6c9fa482f5054e2734d369acf041b18
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118604"
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

