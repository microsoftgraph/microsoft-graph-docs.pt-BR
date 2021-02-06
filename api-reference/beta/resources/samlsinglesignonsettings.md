---
title: Tipo de recurso samlSingleSignOnSettings
description: Representa as configurações de login único do SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 0b82f334196bcd9f7799a3a7a3ef7b5374571ac4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136125"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="64d2b-103">Tipo de recurso samlSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="64d2b-103">samlSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64d2b-104">Representa um contêiner para configurações relacionadas ao single sign-on do SAML.</span><span class="sxs-lookup"><span data-stu-id="64d2b-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="64d2b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64d2b-105">Properties</span></span>

| <span data-ttu-id="64d2b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64d2b-106">Property</span></span> | <span data-ttu-id="64d2b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="64d2b-107">Type</span></span> | <span data-ttu-id="64d2b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="64d2b-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="64d2b-109">relayState</span><span class="sxs-lookup"><span data-stu-id="64d2b-109">relayState</span></span>|<span data-ttu-id="64d2b-110">String</span><span class="sxs-lookup"><span data-stu-id="64d2b-110">String</span></span>| <span data-ttu-id="64d2b-111">O URI relativo ao que o provedor de serviços redirecionaria após a conclusão do fluxo de logom único.</span><span class="sxs-lookup"><span data-stu-id="64d2b-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="64d2b-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64d2b-112">JSON representation</span></span>
<span data-ttu-id="64d2b-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64d2b-113">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
}-->

```json
{
    "relayState": "string",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "samlSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


