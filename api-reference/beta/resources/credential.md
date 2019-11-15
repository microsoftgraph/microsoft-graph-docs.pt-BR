---
title: tipo de recurso Credential
description: Indica uma única credencial usada para entrar em um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3b23249d7c0b898344113c5bcfe950c207891250
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658881"
---
# <a name="credential-resource-type"></a><span data-ttu-id="9753a-103">tipo de recurso Credential</span><span class="sxs-lookup"><span data-stu-id="9753a-103">credential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9753a-104">Indica uma única credencial usada para entrar em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9753a-104">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="9753a-105">Por exemplo, username é uma credencial, password é outra credencial.</span><span class="sxs-lookup"><span data-stu-id="9753a-105">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="9753a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9753a-106">Properties</span></span>

| <span data-ttu-id="9753a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9753a-107">Property</span></span>     | <span data-ttu-id="9753a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9753a-108">Type</span></span>        | <span data-ttu-id="9753a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9753a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9753a-110">fieldId</span><span class="sxs-lookup"><span data-stu-id="9753a-110">fieldId</span></span>|<span data-ttu-id="9753a-111">String</span><span class="sxs-lookup"><span data-stu-id="9753a-111">String</span></span>|<span data-ttu-id="9753a-112">O nome do campo para esta credencial.</span><span class="sxs-lookup"><span data-stu-id="9753a-112">The name of the field for this credential.</span></span> <span data-ttu-id="9753a-113">por exemplo, nome de usuário ou senha ou phoneNumber.</span><span class="sxs-lookup"><span data-stu-id="9753a-113">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="9753a-114">Isso é definido pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9753a-114">This is defined by the application.</span></span> <span data-ttu-id="9753a-115">Deve corresponder ao que está no campo HTML no objeto singleSignOnSettings/password.</span><span class="sxs-lookup"><span data-stu-id="9753a-115">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="9753a-116">type</span><span class="sxs-lookup"><span data-stu-id="9753a-116">type</span></span>|<span data-ttu-id="9753a-117">String</span><span class="sxs-lookup"><span data-stu-id="9753a-117">String</span></span>|<span data-ttu-id="9753a-118">O tipo desta credencial.</span><span class="sxs-lookup"><span data-stu-id="9753a-118">The type for this credential.</span></span> <span data-ttu-id="9753a-119">Valores válidos: username, password ou Other.</span><span class="sxs-lookup"><span data-stu-id="9753a-119">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="9753a-120">value</span><span class="sxs-lookup"><span data-stu-id="9753a-120">value</span></span>|<span data-ttu-id="9753a-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9753a-121">String</span></span>|<span data-ttu-id="9753a-122">O valor dessa credencial.</span><span class="sxs-lookup"><span data-stu-id="9753a-122">The value for this credential.</span></span> <span data-ttu-id="9753a-123">por exemplo, mysuperhiddenpassword.</span><span class="sxs-lookup"><span data-stu-id="9753a-123">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="9753a-124">Observação o valor de senhas é somente gravação, o valor nunca pode ser lido novamente.</span><span class="sxs-lookup"><span data-stu-id="9753a-124">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9753a-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9753a-125">JSON representation</span></span>

<span data-ttu-id="9753a-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9753a-126">The following is a JSON representation of the resource.</span></span>

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
