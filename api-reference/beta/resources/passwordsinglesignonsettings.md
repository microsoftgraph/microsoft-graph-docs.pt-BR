---
title: tipo de recurso passwordSingleSignOnSettings
description: Configurações relacionadas ao logon único baseado em senha
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a1b2739ecbd5d09358e58203ab61d4e65c48716b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998170"
---
# <a name="passwordsinglesignonsettings-resource-type"></a><span data-ttu-id="cba3f-103">tipo de recurso passwordSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="cba3f-103">passwordSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cba3f-104">Contém a coleção de configurações de logon único baseadas em senha.</span><span class="sxs-lookup"><span data-stu-id="cba3f-104">Contains the collection of Password-based single sign-on settings.</span></span>

## <a name="properties"></a><span data-ttu-id="cba3f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cba3f-105">Properties</span></span>

| <span data-ttu-id="cba3f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cba3f-106">Property</span></span>     | <span data-ttu-id="cba3f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cba3f-107">Type</span></span>        | <span data-ttu-id="cba3f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cba3f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cba3f-109">campos</span><span class="sxs-lookup"><span data-stu-id="cba3f-109">fields</span></span>|<span data-ttu-id="cba3f-110">coleção [passwordSingleSignOnField](passwordsinglesignonfield.md)</span><span class="sxs-lookup"><span data-stu-id="cba3f-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) collection</span></span>||

## <a name="json-representation"></a><span data-ttu-id="cba3f-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cba3f-111">JSON representation</span></span>

<span data-ttu-id="cba3f-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cba3f-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnSettings",
  "baseType": null
}-->

```json
{
  "fields": [{"@odata.type": "microsoft.graph.passwordSingleSignOnField"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

