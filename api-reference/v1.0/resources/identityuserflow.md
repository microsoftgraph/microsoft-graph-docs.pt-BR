---
title: Tipo de recurso UserFlow
description: Representa um fluxo de usuário de identidade incluído em uma jornada de autenticação interna.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4e03faaff265bf82bacf16a2db6c75e81176eafa
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882747"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="04701-103">Tipo de recurso UserFlow</span><span class="sxs-lookup"><span data-stu-id="04701-103">UserFlow resource type</span></span>

<span data-ttu-id="04701-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04701-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04701-105">Fluxos de usuário permitem definir políticas predefinidas e configuráveis para entrada, entrada, entrada combinada e entrada, redefinição de senha e atualização de perfil.</span><span class="sxs-lookup"><span data-stu-id="04701-105">User Flows enable you to define predefined, configurable policies for sign-in, sign-up, combined sign-up and sign-in, password reset, and profile update.</span></span> <span data-ttu-id="04701-106">Esta é uma classe base da que outros fluxos de usuário herdam.</span><span class="sxs-lookup"><span data-stu-id="04701-106">This is a base class that other user flows inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="04701-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04701-107">Properties</span></span>

| <span data-ttu-id="04701-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04701-108">Property</span></span>     | <span data-ttu-id="04701-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="04701-109">Type</span></span>        | <span data-ttu-id="04701-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="04701-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04701-111">id</span><span class="sxs-lookup"><span data-stu-id="04701-111">id</span></span>|<span data-ttu-id="04701-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04701-112">String</span></span>| <span data-ttu-id="04701-113">O identificador do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="04701-113">The identifier of the user flow.</span></span> <span data-ttu-id="04701-114">O prefixo **de B2C_1_** é adicionado ao valor que você fornece.</span><span class="sxs-lookup"><span data-stu-id="04701-114">The prefix of **B2C_1_** is added to the value that you provide.</span></span>|
|<span data-ttu-id="04701-115">userFlowType</span><span class="sxs-lookup"><span data-stu-id="04701-115">userFlowType</span></span>|<span data-ttu-id="04701-116">userFlowType</span><span class="sxs-lookup"><span data-stu-id="04701-116">userFlowType</span></span>| <span data-ttu-id="04701-117">Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="04701-117">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="04701-118">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="04701-118">userFlowTypeVersion</span></span>|<span data-ttu-id="04701-119">Único</span><span class="sxs-lookup"><span data-stu-id="04701-119">Single</span></span>| <span data-ttu-id="04701-120">Esta é a versão do tipo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="04701-120">This is the version of the user flow type.</span></span> <span data-ttu-id="04701-121">Cada tipo de fluxo de usuário pode ter diferentes versões possíveis, como 1, 1.1 ou 2.</span><span class="sxs-lookup"><span data-stu-id="04701-121">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="04701-122">Relações</span><span class="sxs-lookup"><span data-stu-id="04701-122">Relationships</span></span>

<span data-ttu-id="04701-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04701-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04701-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04701-124">JSON representation</span></span>

<span data-ttu-id="04701-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04701-125">The following is a JSON representation of the resource.</span></span>

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
