---
title: Tipo de recurso keyValue
description: Fornece informações relevantes adicionais sobre a solicitação de login
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3459f827f35049b383e732c805d61371577b2260
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135391"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="1ef60-103">Tipo de recurso keyValue</span><span class="sxs-lookup"><span data-stu-id="1ef60-103">keyValue resource type</span></span>

<span data-ttu-id="1ef60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ef60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ef60-105">Fornece informações adicionais de processamento de autenticação, como o nome do servidor e a presença de dicas para entrar e domínio.</span><span class="sxs-lookup"><span data-stu-id="1ef60-105">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="1ef60-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ef60-106">Properties</span></span>

| <span data-ttu-id="1ef60-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ef60-107">Property</span></span>     | <span data-ttu-id="1ef60-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ef60-108">Type</span></span>        | <span data-ttu-id="1ef60-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ef60-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1ef60-110">key</span><span class="sxs-lookup"><span data-stu-id="1ef60-110">key</span></span>|<span data-ttu-id="1ef60-111">String</span><span class="sxs-lookup"><span data-stu-id="1ef60-111">String</span></span>|<span data-ttu-id="1ef60-112">Contém o nome do campo ao que um valor está associado.</span><span class="sxs-lookup"><span data-stu-id="1ef60-112">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="1ef60-113">Quando uma dica de login ou domínio é incluída na solicitação de login, os campos correspondentes são incluídos como pares chave-valor.</span><span class="sxs-lookup"><span data-stu-id="1ef60-113">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="1ef60-114">Chaves possíveis: `Login hint present` , `Domain hint present` .</span><span class="sxs-lookup"><span data-stu-id="1ef60-114">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="1ef60-115">value</span><span class="sxs-lookup"><span data-stu-id="1ef60-115">value</span></span>|<span data-ttu-id="1ef60-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ef60-116">String</span></span>|<span data-ttu-id="1ef60-117">Contém o valor correspondente para a chave especificada.</span><span class="sxs-lookup"><span data-stu-id="1ef60-117">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="1ef60-118">O valor é `true` se uma dica de login foi incluída na solicitação de login; caso `false` contrário.</span><span class="sxs-lookup"><span data-stu-id="1ef60-118">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="1ef60-119">O valor é `true` se uma dica de domínio foi incluída na solicitação de login; caso `false` contrário.</span><span class="sxs-lookup"><span data-stu-id="1ef60-119">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ef60-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ef60-120">JSON representation</span></span>

<span data-ttu-id="1ef60-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ef60-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue",
  "baseType": null
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


