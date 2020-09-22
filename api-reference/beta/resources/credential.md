---
title: tipo de recurso Credential
description: Indica uma única credencial usada para entrar em um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a281e39850ea18ee3bcbe0d83c5df3b41d0ccd31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016685"
---
# <a name="credential-resource-type"></a><span data-ttu-id="1d8af-103">tipo de recurso Credential</span><span class="sxs-lookup"><span data-stu-id="1d8af-103">credential resource type</span></span>

<span data-ttu-id="1d8af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d8af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d8af-105">Indica uma única credencial usada para entrar em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d8af-105">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="1d8af-106">Por exemplo, username é uma credencial, password é outra credencial.</span><span class="sxs-lookup"><span data-stu-id="1d8af-106">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="1d8af-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d8af-107">Properties</span></span>

| <span data-ttu-id="1d8af-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d8af-108">Property</span></span>     | <span data-ttu-id="1d8af-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d8af-109">Type</span></span>        | <span data-ttu-id="1d8af-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d8af-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d8af-111">fieldId</span><span class="sxs-lookup"><span data-stu-id="1d8af-111">fieldId</span></span>|<span data-ttu-id="1d8af-112">String</span><span class="sxs-lookup"><span data-stu-id="1d8af-112">String</span></span>|<span data-ttu-id="1d8af-113">O nome do campo para esta credencial.</span><span class="sxs-lookup"><span data-stu-id="1d8af-113">The name of the field for this credential.</span></span> <span data-ttu-id="1d8af-114">por exemplo, nome de usuário ou senha ou phoneNumber.</span><span class="sxs-lookup"><span data-stu-id="1d8af-114">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="1d8af-115">Isso é definido pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d8af-115">This is defined by the application.</span></span> <span data-ttu-id="1d8af-116">Deve corresponder ao que está no campo HTML no objeto singleSignOnSettings/password.</span><span class="sxs-lookup"><span data-stu-id="1d8af-116">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="1d8af-117">tipo</span><span class="sxs-lookup"><span data-stu-id="1d8af-117">type</span></span>|<span data-ttu-id="1d8af-118">String</span><span class="sxs-lookup"><span data-stu-id="1d8af-118">String</span></span>|<span data-ttu-id="1d8af-119">O tipo desta credencial.</span><span class="sxs-lookup"><span data-stu-id="1d8af-119">The type for this credential.</span></span> <span data-ttu-id="1d8af-120">Valores válidos: username, password ou Other.</span><span class="sxs-lookup"><span data-stu-id="1d8af-120">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="1d8af-121">value</span><span class="sxs-lookup"><span data-stu-id="1d8af-121">value</span></span>|<span data-ttu-id="1d8af-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d8af-122">String</span></span>|<span data-ttu-id="1d8af-123">O valor dessa credencial.</span><span class="sxs-lookup"><span data-stu-id="1d8af-123">The value for this credential.</span></span> <span data-ttu-id="1d8af-124">por exemplo, mysuperhiddenpassword.</span><span class="sxs-lookup"><span data-stu-id="1d8af-124">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="1d8af-125">Observação o valor de senhas é somente gravação, o valor nunca pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="1d8af-125">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d8af-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d8af-126">JSON representation</span></span>

<span data-ttu-id="1d8af-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d8af-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credential",
  "baseType": null
}-->

```json
{
  "fieldId": "param_username",
  "value": "myusername",
  "type": "username"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


