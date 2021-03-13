---
title: Tipo de recurso passwordSingleSignOnSettings
description: Configurações relacionadas ao login único baseado em senha
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3e7e4402e6416166dd7c288cdd9aa9ec5ecbba06
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761539"
---
# <a name="passwordsinglesignonsettings-resource-type"></a><span data-ttu-id="a95c4-103">Tipo de recurso passwordSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a95c4-103">passwordSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a95c4-104">Contém a coleção de configurações de login único baseada em senha.</span><span class="sxs-lookup"><span data-stu-id="a95c4-104">Contains the collection of Password-based single sign-on settings.</span></span>

## <a name="properties"></a><span data-ttu-id="a95c4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a95c4-105">Properties</span></span>

| <span data-ttu-id="a95c4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a95c4-106">Property</span></span>     | <span data-ttu-id="a95c4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a95c4-107">Type</span></span>        | <span data-ttu-id="a95c4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a95c4-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a95c4-109">campos</span><span class="sxs-lookup"><span data-stu-id="a95c4-109">fields</span></span>|<span data-ttu-id="a95c4-110">[Coleção passwordSingleSignOnField](passwordsinglesignonfield.md)</span><span class="sxs-lookup"><span data-stu-id="a95c4-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) collection</span></span>||

## <a name="json-representation"></a><span data-ttu-id="a95c4-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a95c4-111">JSON representation</span></span>

<span data-ttu-id="a95c4-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a95c4-112">The following is a JSON representation of the resource.</span></span>

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

