---
title: Tipo de recurso userflow
description: Os fluxos de usuário de identidade são viagens de autenticação integradas
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4fa3064d19d96a2a8297f72de6a625ee36c8db3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496548"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="78d5b-103">Tipo de recurso userflow</span><span class="sxs-lookup"><span data-stu-id="78d5b-103">UserFlow resource type</span></span>

<span data-ttu-id="78d5b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="78d5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78d5b-105">Os fluxos de usuário permitem que você defina políticas configuráveis e predefinidas para entrar, inscrever-se, inscrever-se e entrar, redefinição de senha e atualização de perfil.</span><span class="sxs-lookup"><span data-stu-id="78d5b-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="78d5b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="78d5b-106">Methods</span></span>

| <span data-ttu-id="78d5b-107">Método</span><span class="sxs-lookup"><span data-stu-id="78d5b-107">Method</span></span>       | <span data-ttu-id="78d5b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="78d5b-108">Return Type</span></span> | <span data-ttu-id="78d5b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="78d5b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="78d5b-110">List</span><span class="sxs-lookup"><span data-stu-id="78d5b-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="78d5b-111">Coleção [Userflow](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="78d5b-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="78d5b-112">Listar transflows.</span><span class="sxs-lookup"><span data-stu-id="78d5b-112">List UserFlows.</span></span> |
| [<span data-ttu-id="78d5b-113">Create</span><span class="sxs-lookup"><span data-stu-id="78d5b-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="78d5b-114">Userflow</span><span class="sxs-lookup"><span data-stu-id="78d5b-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="78d5b-115">Criar objeto userflow.</span><span class="sxs-lookup"><span data-stu-id="78d5b-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="78d5b-116">Get</span><span class="sxs-lookup"><span data-stu-id="78d5b-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="78d5b-117">Userflow</span><span class="sxs-lookup"><span data-stu-id="78d5b-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="78d5b-118">Leia as propriedades e as relações do objeto userflow.</span><span class="sxs-lookup"><span data-stu-id="78d5b-118">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="78d5b-119">Delete</span><span class="sxs-lookup"><span data-stu-id="78d5b-119">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="78d5b-120">None</span><span class="sxs-lookup"><span data-stu-id="78d5b-120">None</span></span> | <span data-ttu-id="78d5b-121">Exclua o objeto userflow.</span><span class="sxs-lookup"><span data-stu-id="78d5b-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="78d5b-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78d5b-122">Properties</span></span>

| <span data-ttu-id="78d5b-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78d5b-123">Property</span></span>     | <span data-ttu-id="78d5b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="78d5b-124">Type</span></span>        | <span data-ttu-id="78d5b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="78d5b-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="78d5b-126">id</span><span class="sxs-lookup"><span data-stu-id="78d5b-126">id</span></span>|<span data-ttu-id="78d5b-127">String</span><span class="sxs-lookup"><span data-stu-id="78d5b-127">String</span></span>| <span data-ttu-id="78d5b-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78d5b-128">Read-only.</span></span>|
|<span data-ttu-id="78d5b-129">userflowtype</span><span class="sxs-lookup"><span data-stu-id="78d5b-129">userFlowType</span></span>|<span data-ttu-id="78d5b-130">string</span><span class="sxs-lookup"><span data-stu-id="78d5b-130">string</span></span>| <span data-ttu-id="78d5b-131">Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="78d5b-131">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="78d5b-132">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="78d5b-132">userFlowTypeVersion</span></span>|<span data-ttu-id="78d5b-133">Único</span><span class="sxs-lookup"><span data-stu-id="78d5b-133">Single</span></span>| <span data-ttu-id="78d5b-134">Esta é a versão do tipo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="78d5b-134">This is the version of the user flow type.</span></span> <span data-ttu-id="78d5b-135">Cada tipo de fluxo de usuário pode ter diferentes versões possíveis, como 1, 1,1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="78d5b-135">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="78d5b-136">Relações</span><span class="sxs-lookup"><span data-stu-id="78d5b-136">Relationships</span></span>

<span data-ttu-id="78d5b-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78d5b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78d5b-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78d5b-138">JSON representation</span></span>

<span data-ttu-id="78d5b-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78d5b-139">The following is a JSON representation of the resource.</span></span>

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
