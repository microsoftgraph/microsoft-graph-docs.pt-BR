---
title: Tipo de recurso UserFlow
description: Os fluxos de identidade do usuário são jornadas de autenticação internas
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa6829d346fc1e2520fb5eab28f5ce5fd9c72ae4
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176966"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="3bfec-103">Tipo de recurso UserFlow</span><span class="sxs-lookup"><span data-stu-id="3bfec-103">UserFlow resource type</span></span>

<span data-ttu-id="3bfec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bfec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bfec-105">Os Fluxos de Usuário permitem definir políticas predefinidas e configuráveis para entrar, inscrever-se, se inscrever e entrar combinados, redefinição de senha e atualização de perfil.</span><span class="sxs-lookup"><span data-stu-id="3bfec-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="3bfec-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3bfec-106">Methods</span></span>

| <span data-ttu-id="3bfec-107">Método</span><span class="sxs-lookup"><span data-stu-id="3bfec-107">Method</span></span>       | <span data-ttu-id="3bfec-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3bfec-108">Return Type</span></span> | <span data-ttu-id="3bfec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bfec-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3bfec-110">List</span><span class="sxs-lookup"><span data-stu-id="3bfec-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="3bfec-111">[Coleção UserFlow](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="3bfec-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="3bfec-112">Listar UserFlows.</span><span class="sxs-lookup"><span data-stu-id="3bfec-112">List UserFlows.</span></span> |
| [<span data-ttu-id="3bfec-113">Criar</span><span class="sxs-lookup"><span data-stu-id="3bfec-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="3bfec-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="3bfec-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="3bfec-115">Crie um objeto UserFlow.</span><span class="sxs-lookup"><span data-stu-id="3bfec-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="3bfec-116">Get</span><span class="sxs-lookup"><span data-stu-id="3bfec-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="3bfec-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="3bfec-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="3bfec-118">Leia as propriedades e os relacionamentos do objeto UserFlow.</span><span class="sxs-lookup"><span data-stu-id="3bfec-118">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="3bfec-119">Delete</span><span class="sxs-lookup"><span data-stu-id="3bfec-119">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="3bfec-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bfec-120">None</span></span> | <span data-ttu-id="3bfec-121">Exclua o objeto UserFlow.</span><span class="sxs-lookup"><span data-stu-id="3bfec-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3bfec-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bfec-122">Properties</span></span>

| <span data-ttu-id="3bfec-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bfec-123">Property</span></span>     | <span data-ttu-id="3bfec-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bfec-124">Type</span></span>        | <span data-ttu-id="3bfec-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bfec-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3bfec-126">id</span><span class="sxs-lookup"><span data-stu-id="3bfec-126">id</span></span>|<span data-ttu-id="3bfec-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bfec-127">String</span></span>| <span data-ttu-id="3bfec-128">O identificador do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="3bfec-128">The identifier of the user flow.</span></span> <span data-ttu-id="3bfec-129">O prefixo **B2C_1_** é adicionado ao valor que você fornece.</span><span class="sxs-lookup"><span data-stu-id="3bfec-129">The prefix of **B2C_1_** is added to the value that you provide.</span></span>|
|<span data-ttu-id="3bfec-130">userFlowType</span><span class="sxs-lookup"><span data-stu-id="3bfec-130">userFlowType</span></span>|<span data-ttu-id="3bfec-131">string</span><span class="sxs-lookup"><span data-stu-id="3bfec-131">string</span></span>| <span data-ttu-id="3bfec-132">Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3bfec-132">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3bfec-133">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="3bfec-133">userFlowTypeVersion</span></span>|<span data-ttu-id="3bfec-134">Único</span><span class="sxs-lookup"><span data-stu-id="3bfec-134">Single</span></span>| <span data-ttu-id="3bfec-135">Esta é a versão do tipo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="3bfec-135">This is the version of the user flow type.</span></span> <span data-ttu-id="3bfec-136">Cada tipo de fluxo de usuário pode ter diferentes versões possíveis, como 1, 1.1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="3bfec-136">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="3bfec-137">Relações</span><span class="sxs-lookup"><span data-stu-id="3bfec-137">Relationships</span></span>

<span data-ttu-id="3bfec-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bfec-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bfec-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bfec-139">JSON representation</span></span>

<span data-ttu-id="3bfec-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bfec-140">The following is a JSON representation of the resource.</span></span>

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


