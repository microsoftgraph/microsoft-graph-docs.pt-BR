---
title: tipo de recurso samlSingleSignOnSettings
description: Representa as configurações de logon único do SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 6c07e9c0284ef111a3032ec729c3b741be65f920
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016027"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="b180d-103">tipo de recurso samlSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="b180d-103">samlSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b180d-104">Representa um contêiner para configurações relacionadas ao logon único do SAML.</span><span class="sxs-lookup"><span data-stu-id="b180d-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="b180d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b180d-105">Properties</span></span>

| <span data-ttu-id="b180d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b180d-106">Property</span></span> | <span data-ttu-id="b180d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b180d-107">Type</span></span> | <span data-ttu-id="b180d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b180d-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b180d-109">relaystate</span><span class="sxs-lookup"><span data-stu-id="b180d-109">relayState</span></span>|<span data-ttu-id="b180d-110">String</span><span class="sxs-lookup"><span data-stu-id="b180d-110">String</span></span>| <span data-ttu-id="b180d-111">O URI relativo para o qual o provedor de serviços redirecionaria após a conclusão do fluxo de logon único.</span><span class="sxs-lookup"><span data-stu-id="b180d-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b180d-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b180d-112">JSON representation</span></span>
<span data-ttu-id="b180d-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b180d-113">Here is a JSON representation of the resource.</span></span>

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


