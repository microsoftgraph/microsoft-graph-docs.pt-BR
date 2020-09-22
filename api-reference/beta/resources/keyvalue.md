---
title: tipo de recurso KeyValue
description: Fornece informações relevantes adicionais sobre a solicitação de entrada
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0a25d9c69b3495bcc2efc38b3e87b373f247d024
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078337"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="eb79c-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="eb79c-103">keyValue resource type</span></span>

<span data-ttu-id="eb79c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb79c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb79c-105">Fornece informações de processamento de autenticação adicionais, como o nome do servidor e a presença de dicas para entrar e domínio.</span><span class="sxs-lookup"><span data-stu-id="eb79c-105">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="eb79c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb79c-106">Properties</span></span>

| <span data-ttu-id="eb79c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb79c-107">Property</span></span>     | <span data-ttu-id="eb79c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb79c-108">Type</span></span>        | <span data-ttu-id="eb79c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb79c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb79c-110">key</span><span class="sxs-lookup"><span data-stu-id="eb79c-110">key</span></span>|<span data-ttu-id="eb79c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb79c-111">String</span></span>|<span data-ttu-id="eb79c-112">Contém o nome do campo ao qual um valor está associado.</span><span class="sxs-lookup"><span data-stu-id="eb79c-112">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="eb79c-113">Quando uma dica de entrada ou de domínio é incluída na solicitação de entrada, os campos correspondentes são incluídos como pares de chave-valor.</span><span class="sxs-lookup"><span data-stu-id="eb79c-113">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="eb79c-114">Chaves possíveis: `Login hint present` , `Domain hint present` .</span><span class="sxs-lookup"><span data-stu-id="eb79c-114">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="eb79c-115">value</span><span class="sxs-lookup"><span data-stu-id="eb79c-115">value</span></span>|<span data-ttu-id="eb79c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb79c-116">String</span></span>|<span data-ttu-id="eb79c-117">Contém o valor correspondente para a chave especificada.</span><span class="sxs-lookup"><span data-stu-id="eb79c-117">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="eb79c-118">O valor é `true` se uma dica de entrada foi incluída na solicitação de entrada; caso contrário `false` .</span><span class="sxs-lookup"><span data-stu-id="eb79c-118">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="eb79c-119">O valor é `true` se uma dica de domínio foi incluída na solicitação de entrada; caso contrário `false` .</span><span class="sxs-lookup"><span data-stu-id="eb79c-119">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb79c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb79c-120">JSON representation</span></span>

<span data-ttu-id="eb79c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb79c-121">The following is a JSON representation of the resource.</span></span>

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


