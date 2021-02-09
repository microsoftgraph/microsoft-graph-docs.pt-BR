---
title: Tipo de recurso UserFlow
description: Os fluxos de identidade do usuário são jornadas de autenticação internas
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b4842b506e3c3c3e675ec2a47837fbf0c2e10be
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158286"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="82fb7-103">Tipo de recurso UserFlow</span><span class="sxs-lookup"><span data-stu-id="82fb7-103">UserFlow resource type</span></span>

<span data-ttu-id="82fb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82fb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82fb7-105">Os Fluxos de Usuário permitem definir políticas predefinidas e configuráveis para entrar, inscrever-se, se inscrever e entrar combinados, redefinição de senha e atualização de perfil.</span><span class="sxs-lookup"><span data-stu-id="82fb7-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="82fb7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="82fb7-106">Methods</span></span>

| <span data-ttu-id="82fb7-107">Método</span><span class="sxs-lookup"><span data-stu-id="82fb7-107">Method</span></span>       | <span data-ttu-id="82fb7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="82fb7-108">Return Type</span></span> | <span data-ttu-id="82fb7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="82fb7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="82fb7-110">List</span><span class="sxs-lookup"><span data-stu-id="82fb7-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="82fb7-111">[Coleção UserFlow](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="82fb7-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="82fb7-112">Listar UserFlows.</span><span class="sxs-lookup"><span data-stu-id="82fb7-112">List UserFlows.</span></span> |
| [<span data-ttu-id="82fb7-113">Criar</span><span class="sxs-lookup"><span data-stu-id="82fb7-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="82fb7-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="82fb7-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="82fb7-115">Crie um objeto UserFlow.</span><span class="sxs-lookup"><span data-stu-id="82fb7-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="82fb7-116">Get</span><span class="sxs-lookup"><span data-stu-id="82fb7-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="82fb7-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="82fb7-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="82fb7-118">Leia as propriedades e os relacionamentos do objeto UserFlow.</span><span class="sxs-lookup"><span data-stu-id="82fb7-118">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="82fb7-119">Delete</span><span class="sxs-lookup"><span data-stu-id="82fb7-119">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="82fb7-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="82fb7-120">None</span></span> | <span data-ttu-id="82fb7-121">Exclua o objeto UserFlow.</span><span class="sxs-lookup"><span data-stu-id="82fb7-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="82fb7-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82fb7-122">Properties</span></span>

| <span data-ttu-id="82fb7-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82fb7-123">Property</span></span>     | <span data-ttu-id="82fb7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="82fb7-124">Type</span></span>        | <span data-ttu-id="82fb7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="82fb7-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="82fb7-126">id</span><span class="sxs-lookup"><span data-stu-id="82fb7-126">id</span></span>|<span data-ttu-id="82fb7-127">String</span><span class="sxs-lookup"><span data-stu-id="82fb7-127">String</span></span>| <span data-ttu-id="82fb7-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82fb7-128">Read-only.</span></span>|
|<span data-ttu-id="82fb7-129">userFlowType</span><span class="sxs-lookup"><span data-stu-id="82fb7-129">userFlowType</span></span>|<span data-ttu-id="82fb7-130">string</span><span class="sxs-lookup"><span data-stu-id="82fb7-130">string</span></span>| <span data-ttu-id="82fb7-131">Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="82fb7-131">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="82fb7-132">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="82fb7-132">userFlowTypeVersion</span></span>|<span data-ttu-id="82fb7-133">Único</span><span class="sxs-lookup"><span data-stu-id="82fb7-133">Single</span></span>| <span data-ttu-id="82fb7-134">Esta é a versão do tipo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="82fb7-134">This is the version of the user flow type.</span></span> <span data-ttu-id="82fb7-135">Cada tipo de fluxo de usuário pode ter diferentes versões possíveis, como 1, 1.1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="82fb7-135">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="82fb7-136">Relações</span><span class="sxs-lookup"><span data-stu-id="82fb7-136">Relationships</span></span>

<span data-ttu-id="82fb7-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82fb7-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82fb7-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82fb7-138">JSON representation</span></span>

<span data-ttu-id="82fb7-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82fb7-139">The following is a JSON representation of the resource.</span></span>

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


