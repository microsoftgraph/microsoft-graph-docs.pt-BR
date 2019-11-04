---
title: tipo de recurso KeyValue
description: Fornece informações relevantes adicionais sobre a solicitação de entrada
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 08f9fc138710626a5b8c1c2b11eeab8ed4cad673
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939303"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="c0d82-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="c0d82-103">keyValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0d82-104">Fornece informações de processamento de autenticação adicionais, como o nome do servidor e a presença de dicas para entrar e domínio.</span><span class="sxs-lookup"><span data-stu-id="c0d82-104">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="c0d82-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0d82-105">Properties</span></span>

| <span data-ttu-id="c0d82-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0d82-106">Property</span></span>     | <span data-ttu-id="c0d82-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0d82-107">Type</span></span>        | <span data-ttu-id="c0d82-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0d82-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0d82-109">key</span><span class="sxs-lookup"><span data-stu-id="c0d82-109">key</span></span>|<span data-ttu-id="c0d82-110">String</span><span class="sxs-lookup"><span data-stu-id="c0d82-110">String</span></span>|<span data-ttu-id="c0d82-111">Contém o nome do campo ao qual um valor está associado.</span><span class="sxs-lookup"><span data-stu-id="c0d82-111">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="c0d82-112">Quando uma dica de entrada ou de domínio é incluída na solicitação de entrada, os campos correspondentes são incluídos como pares de chave-valor.</span><span class="sxs-lookup"><span data-stu-id="c0d82-112">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="c0d82-113">Chaves possíveis: `Login hint present`, `Domain hint present`.</span><span class="sxs-lookup"><span data-stu-id="c0d82-113">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="c0d82-114">value</span><span class="sxs-lookup"><span data-stu-id="c0d82-114">value</span></span>|<span data-ttu-id="c0d82-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0d82-115">String</span></span>|<span data-ttu-id="c0d82-116">Contém o valor correspondente para a chave especificada.</span><span class="sxs-lookup"><span data-stu-id="c0d82-116">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="c0d82-117">O valor é `true` se uma dica de entrada foi incluída na solicitação de entrada; caso `false`contrário.</span><span class="sxs-lookup"><span data-stu-id="c0d82-117">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="c0d82-118">O valor é `true` se uma dica de domínio foi incluída na solicitação de entrada; caso `false`contrário.</span><span class="sxs-lookup"><span data-stu-id="c0d82-118">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0d82-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0d82-119">JSON representation</span></span>

<span data-ttu-id="c0d82-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0d82-120">The following is a JSON representation of the resource.</span></span>

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
