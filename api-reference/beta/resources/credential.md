---
title: tipo de recurso de credencial
description: Indica uma única credencial usada para entrar em um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0521f766a7a0da482cf67628c3816935ee9270b8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761678"
---
# <a name="credential-resource-type"></a><span data-ttu-id="e9930-103">tipo de recurso de credencial</span><span class="sxs-lookup"><span data-stu-id="e9930-103">credential resource type</span></span>

<span data-ttu-id="e9930-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9930-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9930-105">Indica uma única credencial usada para entrar em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e9930-105">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="e9930-106">Por exemplo, nome de usuário é uma credencial, senha é outra credencial.</span><span class="sxs-lookup"><span data-stu-id="e9930-106">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="e9930-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9930-107">Properties</span></span>

| <span data-ttu-id="e9930-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9930-108">Property</span></span>     | <span data-ttu-id="e9930-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9930-109">Type</span></span>        | <span data-ttu-id="e9930-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9930-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9930-111">fieldId</span><span class="sxs-lookup"><span data-stu-id="e9930-111">fieldId</span></span>|<span data-ttu-id="e9930-112">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e9930-112">String</span></span>|<span data-ttu-id="e9930-113">O nome do campo para essa credencial.</span><span class="sxs-lookup"><span data-stu-id="e9930-113">The name of the field for this credential.</span></span> <span data-ttu-id="e9930-114">por exemplo, nome de usuário ou senha ou telefoneNumber.</span><span class="sxs-lookup"><span data-stu-id="e9930-114">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="e9930-115">Isso é definido pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e9930-115">This is defined by the application.</span></span> <span data-ttu-id="e9930-116">Deve corresponder ao que está no campo html no objeto singleSignOnSettings/password.</span><span class="sxs-lookup"><span data-stu-id="e9930-116">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="e9930-117">tipo</span><span class="sxs-lookup"><span data-stu-id="e9930-117">type</span></span>|<span data-ttu-id="e9930-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9930-118">String</span></span>|<span data-ttu-id="e9930-119">O tipo dessa credencial.</span><span class="sxs-lookup"><span data-stu-id="e9930-119">The type for this credential.</span></span> <span data-ttu-id="e9930-120">Valores válidos: nome de usuário, senha ou outros.</span><span class="sxs-lookup"><span data-stu-id="e9930-120">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="e9930-121">value</span><span class="sxs-lookup"><span data-stu-id="e9930-121">value</span></span>|<span data-ttu-id="e9930-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9930-122">String</span></span>|<span data-ttu-id="e9930-123">O valor dessa credencial.</span><span class="sxs-lookup"><span data-stu-id="e9930-123">The value for this credential.</span></span> <span data-ttu-id="e9930-124">por exemplo, mysuperhiddenpassword.</span><span class="sxs-lookup"><span data-stu-id="e9930-124">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="e9930-125">Observe que o valor das senhas é somente gravação, o valor nunca poderá ser lido de volta.</span><span class="sxs-lookup"><span data-stu-id="e9930-125">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9930-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9930-126">JSON representation</span></span>

<span data-ttu-id="e9930-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9930-127">The following is a JSON representation of the resource.</span></span>

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


