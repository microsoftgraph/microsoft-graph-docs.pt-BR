---
title: tipo de recurso Credential
description: Indica uma única credencial usada para entrar em um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c7638c08214002a58328378967c024af871cb734
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507356"
---
# <a name="credential-resource-type"></a><span data-ttu-id="1945e-103">tipo de recurso Credential</span><span class="sxs-lookup"><span data-stu-id="1945e-103">credential resource type</span></span>

<span data-ttu-id="1945e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1945e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1945e-105">Indica uma única credencial usada para entrar em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1945e-105">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="1945e-106">Por exemplo, username é uma credencial, password é outra credencial.</span><span class="sxs-lookup"><span data-stu-id="1945e-106">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="1945e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1945e-107">Properties</span></span>

| <span data-ttu-id="1945e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1945e-108">Property</span></span>     | <span data-ttu-id="1945e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1945e-109">Type</span></span>        | <span data-ttu-id="1945e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1945e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1945e-111">fieldId</span><span class="sxs-lookup"><span data-stu-id="1945e-111">fieldId</span></span>|<span data-ttu-id="1945e-112">String</span><span class="sxs-lookup"><span data-stu-id="1945e-112">String</span></span>|<span data-ttu-id="1945e-113">O nome do campo para esta credencial.</span><span class="sxs-lookup"><span data-stu-id="1945e-113">The name of the field for this credential.</span></span> <span data-ttu-id="1945e-114">por exemplo, nome de usuário ou senha ou phoneNumber.</span><span class="sxs-lookup"><span data-stu-id="1945e-114">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="1945e-115">Isso é definido pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1945e-115">This is defined by the application.</span></span> <span data-ttu-id="1945e-116">Deve corresponder ao que está no campo HTML no objeto singleSignOnSettings/password.</span><span class="sxs-lookup"><span data-stu-id="1945e-116">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="1945e-117">type</span><span class="sxs-lookup"><span data-stu-id="1945e-117">type</span></span>|<span data-ttu-id="1945e-118">String</span><span class="sxs-lookup"><span data-stu-id="1945e-118">String</span></span>|<span data-ttu-id="1945e-119">O tipo desta credencial.</span><span class="sxs-lookup"><span data-stu-id="1945e-119">The type for this credential.</span></span> <span data-ttu-id="1945e-120">Valores válidos: username, password ou Other.</span><span class="sxs-lookup"><span data-stu-id="1945e-120">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="1945e-121">value</span><span class="sxs-lookup"><span data-stu-id="1945e-121">value</span></span>|<span data-ttu-id="1945e-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1945e-122">String</span></span>|<span data-ttu-id="1945e-123">O valor dessa credencial.</span><span class="sxs-lookup"><span data-stu-id="1945e-123">The value for this credential.</span></span> <span data-ttu-id="1945e-124">por exemplo, mysuperhiddenpassword.</span><span class="sxs-lookup"><span data-stu-id="1945e-124">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="1945e-125">Observação o valor de senhas é somente gravação, o valor nunca pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="1945e-125">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1945e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1945e-126">JSON representation</span></span>

<span data-ttu-id="1945e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1945e-127">The following is a JSON representation of the resource.</span></span>

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
