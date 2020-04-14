---
title: tipo de recurso KeyValue
description: Fornece informações relevantes adicionais sobre a solicitação de entrada
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e3f85936e94da0485d62478f54eed8918967396b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442720"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="72a3f-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="72a3f-103">keyValue resource type</span></span>

<span data-ttu-id="72a3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72a3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72a3f-105">Fornece informações de processamento de autenticação adicionais, como o nome do servidor e a presença de dicas para entrar e domínio.</span><span class="sxs-lookup"><span data-stu-id="72a3f-105">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="72a3f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72a3f-106">Properties</span></span>

| <span data-ttu-id="72a3f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72a3f-107">Property</span></span>     | <span data-ttu-id="72a3f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="72a3f-108">Type</span></span>        | <span data-ttu-id="72a3f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="72a3f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="72a3f-110">key</span><span class="sxs-lookup"><span data-stu-id="72a3f-110">key</span></span>|<span data-ttu-id="72a3f-111">String</span><span class="sxs-lookup"><span data-stu-id="72a3f-111">String</span></span>|<span data-ttu-id="72a3f-112">Contém o nome do campo ao qual um valor está associado.</span><span class="sxs-lookup"><span data-stu-id="72a3f-112">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="72a3f-113">Quando uma dica de entrada ou de domínio é incluída na solicitação de entrada, os campos correspondentes são incluídos como pares de chave-valor.</span><span class="sxs-lookup"><span data-stu-id="72a3f-113">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="72a3f-114">Chaves possíveis: `Login hint present`, `Domain hint present`.</span><span class="sxs-lookup"><span data-stu-id="72a3f-114">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="72a3f-115">value</span><span class="sxs-lookup"><span data-stu-id="72a3f-115">value</span></span>|<span data-ttu-id="72a3f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72a3f-116">String</span></span>|<span data-ttu-id="72a3f-117">Contém o valor correspondente para a chave especificada.</span><span class="sxs-lookup"><span data-stu-id="72a3f-117">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="72a3f-118">O valor é `true` se uma dica de entrada foi incluída na solicitação de entrada; caso `false`contrário.</span><span class="sxs-lookup"><span data-stu-id="72a3f-118">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="72a3f-119">O valor é `true` se uma dica de domínio foi incluída na solicitação de entrada; caso `false`contrário.</span><span class="sxs-lookup"><span data-stu-id="72a3f-119">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72a3f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72a3f-120">JSON representation</span></span>

<span data-ttu-id="72a3f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72a3f-121">The following is a JSON representation of the resource.</span></span>

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
