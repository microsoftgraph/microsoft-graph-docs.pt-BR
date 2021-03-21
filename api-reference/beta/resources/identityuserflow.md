---
title: Tipo de recurso UserFlow
description: Fluxos de usuários de identidade são jornadas de autenticação internas
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5401aeb67ccc894e2c151507c0a857b14c3dabb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957020"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="3a33c-103">Tipo de recurso UserFlow</span><span class="sxs-lookup"><span data-stu-id="3a33c-103">UserFlow resource type</span></span>

<span data-ttu-id="3a33c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a33c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a33c-105">Fluxos de usuário permitem definir políticas predefinidas e configuráveis para entrar, se inscrever, se inscrever e entrar combinados, redefinir senha e atualizar o perfil.</span><span class="sxs-lookup"><span data-stu-id="3a33c-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="3a33c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3a33c-106">Methods</span></span>

| <span data-ttu-id="3a33c-107">Método</span><span class="sxs-lookup"><span data-stu-id="3a33c-107">Method</span></span>       | <span data-ttu-id="3a33c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3a33c-108">Return Type</span></span> | <span data-ttu-id="3a33c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a33c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3a33c-110">List</span><span class="sxs-lookup"><span data-stu-id="3a33c-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="3a33c-111">[Coleção UserFlow](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="3a33c-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="3a33c-112">Listar UserFlows.</span><span class="sxs-lookup"><span data-stu-id="3a33c-112">List UserFlows.</span></span> |
| [<span data-ttu-id="3a33c-113">Create</span><span class="sxs-lookup"><span data-stu-id="3a33c-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="3a33c-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="3a33c-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="3a33c-115">Criar objeto UserFlow.</span><span class="sxs-lookup"><span data-stu-id="3a33c-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="3a33c-116">Get</span><span class="sxs-lookup"><span data-stu-id="3a33c-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="3a33c-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="3a33c-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="3a33c-118">Ler propriedades e relações do objeto UserFlow.</span><span class="sxs-lookup"><span data-stu-id="3a33c-118">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="3a33c-119">Delete</span><span class="sxs-lookup"><span data-stu-id="3a33c-119">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="3a33c-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a33c-120">None</span></span> | <span data-ttu-id="3a33c-121">Excluir objeto UserFlow.</span><span class="sxs-lookup"><span data-stu-id="3a33c-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3a33c-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a33c-122">Properties</span></span>

| <span data-ttu-id="3a33c-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a33c-123">Property</span></span>     | <span data-ttu-id="3a33c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a33c-124">Type</span></span>        | <span data-ttu-id="3a33c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a33c-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a33c-126">id</span><span class="sxs-lookup"><span data-stu-id="3a33c-126">id</span></span>|<span data-ttu-id="3a33c-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a33c-127">String</span></span>| <span data-ttu-id="3a33c-128">O identificador do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="3a33c-128">The identifier of the user flow.</span></span> <span data-ttu-id="3a33c-129">O prefixo **de B2C_1_** é adicionado ao valor que você fornece.</span><span class="sxs-lookup"><span data-stu-id="3a33c-129">The prefix of **B2C_1_** is added to the value that you provide.</span></span>|
|<span data-ttu-id="3a33c-130">userFlowType</span><span class="sxs-lookup"><span data-stu-id="3a33c-130">userFlowType</span></span>|<span data-ttu-id="3a33c-131">userFlowType</span><span class="sxs-lookup"><span data-stu-id="3a33c-131">userFlowType</span></span>| <span data-ttu-id="3a33c-132">Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3a33c-132">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3a33c-133">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="3a33c-133">userFlowTypeVersion</span></span>|<span data-ttu-id="3a33c-134">Único</span><span class="sxs-lookup"><span data-stu-id="3a33c-134">Single</span></span>| <span data-ttu-id="3a33c-135">Esta é a versão do tipo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="3a33c-135">This is the version of the user flow type.</span></span> <span data-ttu-id="3a33c-136">Cada tipo de fluxo de usuário pode ter diferentes versões possíveis, como 1, 1.1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="3a33c-136">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="3a33c-137">Relações</span><span class="sxs-lookup"><span data-stu-id="3a33c-137">Relationships</span></span>

<span data-ttu-id="3a33c-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a33c-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a33c-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a33c-139">JSON representation</span></span>

<span data-ttu-id="3a33c-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a33c-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
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


