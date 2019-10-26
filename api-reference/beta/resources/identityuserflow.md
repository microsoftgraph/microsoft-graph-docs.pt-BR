---
title: Tipo de recurso userflow
description: Os fluxos de usuário de identidade são viagens de autenticação integradas
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5410b65dfdb0841aa997022b43dc04d0a4627008
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734506"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="04e1a-103">Tipo de recurso userflow</span><span class="sxs-lookup"><span data-stu-id="04e1a-103">UserFlow resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04e1a-104">Os fluxos de usuário permitem que você defina políticas configuráveis e predefinidas para entrar, inscrever-se, inscrever-se e entrar, redefinição de senha e atualização de perfil.</span><span class="sxs-lookup"><span data-stu-id="04e1a-104">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="04e1a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="04e1a-105">Methods</span></span>

| <span data-ttu-id="04e1a-106">Método</span><span class="sxs-lookup"><span data-stu-id="04e1a-106">Method</span></span>       | <span data-ttu-id="04e1a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="04e1a-107">Return Type</span></span> | <span data-ttu-id="04e1a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="04e1a-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="04e1a-109">List</span><span class="sxs-lookup"><span data-stu-id="04e1a-109">List</span></span>](../api/identityuserflow-list.md) | [<span data-ttu-id="04e1a-110">Userflow</span><span class="sxs-lookup"><span data-stu-id="04e1a-110">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="04e1a-111">Listar transflows.</span><span class="sxs-lookup"><span data-stu-id="04e1a-111">List UserFlows.</span></span> |
| [<span data-ttu-id="04e1a-112">Create</span><span class="sxs-lookup"><span data-stu-id="04e1a-112">Create</span></span>](../api/identityuserflow-post-userflows.md) | <span data-ttu-id="04e1a-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04e1a-113">None</span></span> | <span data-ttu-id="04e1a-114">Criar objeto userflow.</span><span class="sxs-lookup"><span data-stu-id="04e1a-114">Create UserFlow object.</span></span> |
| [<span data-ttu-id="04e1a-115">Get</span><span class="sxs-lookup"><span data-stu-id="04e1a-115">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="04e1a-116">Userflow</span><span class="sxs-lookup"><span data-stu-id="04e1a-116">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="04e1a-117">Leia as propriedades e as relações do objeto userflow.</span><span class="sxs-lookup"><span data-stu-id="04e1a-117">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="04e1a-118">Delete</span><span class="sxs-lookup"><span data-stu-id="04e1a-118">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="04e1a-119">None</span><span class="sxs-lookup"><span data-stu-id="04e1a-119">None</span></span> | <span data-ttu-id="04e1a-120">Exclua o objeto userflow.</span><span class="sxs-lookup"><span data-stu-id="04e1a-120">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="04e1a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04e1a-121">Properties</span></span>

| <span data-ttu-id="04e1a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04e1a-122">Property</span></span>     | <span data-ttu-id="04e1a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="04e1a-123">Type</span></span>        | <span data-ttu-id="04e1a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="04e1a-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04e1a-125">id</span><span class="sxs-lookup"><span data-stu-id="04e1a-125">id</span></span>|<span data-ttu-id="04e1a-126">String</span><span class="sxs-lookup"><span data-stu-id="04e1a-126">String</span></span>| <span data-ttu-id="04e1a-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="04e1a-127">Read-only.</span></span>|
|<span data-ttu-id="04e1a-128">userflowtype</span><span class="sxs-lookup"><span data-stu-id="04e1a-128">userFlowType</span></span>|<span data-ttu-id="04e1a-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04e1a-129">string</span></span>| <span data-ttu-id="04e1a-130">Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="04e1a-130">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="04e1a-131">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="04e1a-131">userFlowTypeVersion</span></span>|<span data-ttu-id="04e1a-132">Único</span><span class="sxs-lookup"><span data-stu-id="04e1a-132">Single</span></span>| <span data-ttu-id="04e1a-133">Esta é a versão do tipo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="04e1a-133">This is the version of the user flow type.</span></span> <span data-ttu-id="04e1a-134">Cada tipo de fluxo de usuário pode ter diferentes versões possíveis, como 1, 1,1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="04e1a-134">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="04e1a-135">Relações</span><span class="sxs-lookup"><span data-stu-id="04e1a-135">Relationships</span></span>

<span data-ttu-id="04e1a-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04e1a-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04e1a-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04e1a-137">JSON representation</span></span>

<span data-ttu-id="04e1a-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04e1a-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "userFlowType": "string",
  "userFlowTypeVersion": "Single"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UserFlow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
