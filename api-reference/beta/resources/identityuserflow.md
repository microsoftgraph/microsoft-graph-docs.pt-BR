---
title: Tipo de recurso userflow
description: Os fluxos de usuário de identidade são viagens de autenticação integradas
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0d76d7a2ab3516717d01f0371b84531e211181fd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016629"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="b40eb-103">Tipo de recurso userflow</span><span class="sxs-lookup"><span data-stu-id="b40eb-103">UserFlow resource type</span></span>

<span data-ttu-id="b40eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b40eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b40eb-105">Os fluxos de usuário permitem que você defina políticas configuráveis e predefinidas para entrar, inscrever-se, inscrever-se e entrar, redefinição de senha e atualização de perfil.</span><span class="sxs-lookup"><span data-stu-id="b40eb-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="b40eb-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b40eb-106">Methods</span></span>

| <span data-ttu-id="b40eb-107">Método</span><span class="sxs-lookup"><span data-stu-id="b40eb-107">Method</span></span>       | <span data-ttu-id="b40eb-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b40eb-108">Return Type</span></span> | <span data-ttu-id="b40eb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b40eb-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b40eb-110">List</span><span class="sxs-lookup"><span data-stu-id="b40eb-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="b40eb-111">Coleção [Userflow](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="b40eb-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="b40eb-112">Listar transflows.</span><span class="sxs-lookup"><span data-stu-id="b40eb-112">List UserFlows.</span></span> |
| [<span data-ttu-id="b40eb-113">Create</span><span class="sxs-lookup"><span data-stu-id="b40eb-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="b40eb-114">Userflow</span><span class="sxs-lookup"><span data-stu-id="b40eb-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="b40eb-115">Criar objeto userflow.</span><span class="sxs-lookup"><span data-stu-id="b40eb-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="b40eb-116">Get</span><span class="sxs-lookup"><span data-stu-id="b40eb-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="b40eb-117">Userflow</span><span class="sxs-lookup"><span data-stu-id="b40eb-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="b40eb-118">Leia as propriedades e as relações do objeto userflow.</span><span class="sxs-lookup"><span data-stu-id="b40eb-118">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="b40eb-119">Delete</span><span class="sxs-lookup"><span data-stu-id="b40eb-119">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="b40eb-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b40eb-120">None</span></span> | <span data-ttu-id="b40eb-121">Exclua o objeto userflow.</span><span class="sxs-lookup"><span data-stu-id="b40eb-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b40eb-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b40eb-122">Properties</span></span>

| <span data-ttu-id="b40eb-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b40eb-123">Property</span></span>     | <span data-ttu-id="b40eb-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b40eb-124">Type</span></span>        | <span data-ttu-id="b40eb-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b40eb-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b40eb-126">id</span><span class="sxs-lookup"><span data-stu-id="b40eb-126">id</span></span>|<span data-ttu-id="b40eb-127">String</span><span class="sxs-lookup"><span data-stu-id="b40eb-127">String</span></span>| <span data-ttu-id="b40eb-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b40eb-128">Read-only.</span></span>|
|<span data-ttu-id="b40eb-129">userFlowType</span><span class="sxs-lookup"><span data-stu-id="b40eb-129">userFlowType</span></span>|<span data-ttu-id="b40eb-130">string</span><span class="sxs-lookup"><span data-stu-id="b40eb-130">string</span></span>| <span data-ttu-id="b40eb-131">Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b40eb-131">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b40eb-132">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="b40eb-132">userFlowTypeVersion</span></span>|<span data-ttu-id="b40eb-133">Único</span><span class="sxs-lookup"><span data-stu-id="b40eb-133">Single</span></span>| <span data-ttu-id="b40eb-134">Esta é a versão do tipo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="b40eb-134">This is the version of the user flow type.</span></span> <span data-ttu-id="b40eb-135">Cada tipo de fluxo de usuário pode ter diferentes versões possíveis, como 1, 1,1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="b40eb-135">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="b40eb-136">Relações</span><span class="sxs-lookup"><span data-stu-id="b40eb-136">Relationships</span></span>

<span data-ttu-id="b40eb-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b40eb-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b40eb-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b40eb-138">JSON representation</span></span>

<span data-ttu-id="b40eb-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b40eb-139">The following is a JSON representation of the resource.</span></span>

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


