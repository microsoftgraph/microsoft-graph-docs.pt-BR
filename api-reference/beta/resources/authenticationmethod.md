---
title: tipo de recurso authenticationMethod
description: Representa um método de autenticação registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9ab808934491793b796be1c66fc87051ed6e9b29
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335622"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="4ecae-103">tipo de recurso authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ecae-103">authenticationMethod resource type</span></span>

<span data-ttu-id="4ecae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ecae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ecae-105">Representa um método de autenticação registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="4ecae-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="4ecae-106">Um [método de autenticação](/azure/active-directory/authentication/concept-authentication-methods) é algo usado por um usuário para autenticar ou provar sua identidade para o sistema.</span><span class="sxs-lookup"><span data-stu-id="4ecae-106">An [authentication method](/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="4ecae-107">Alguns exemplos incluem senha, telefone (que pode ser SMS ou chamada de voz), teclas de segurança FIDO2 e muito mais.</span><span class="sxs-lookup"><span data-stu-id="4ecae-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4ecae-108">Listar os métodos de autenticação dos usuários retorna apenas os métodos suportados nesta versão da API.</span><span class="sxs-lookup"><span data-stu-id="4ecae-108">Listing users' authentication methods only returns methods supported on this API version.</span></span> <span data-ttu-id="4ecae-109">Consulte [Azure AD authentication methods API overview](authenticationmethods-overview.md) for a list of currently supported methods.</span><span class="sxs-lookup"><span data-stu-id="4ecae-109">See [Azure AD authentication methods API overview](authenticationmethods-overview.md) for a list of currently supported methods.</span></span>

## <a name="methods"></a><span data-ttu-id="4ecae-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="4ecae-110">Methods</span></span>

| <span data-ttu-id="4ecae-111">Método</span><span class="sxs-lookup"><span data-stu-id="4ecae-111">Method</span></span>       | <span data-ttu-id="4ecae-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4ecae-112">Return type</span></span> | <span data-ttu-id="4ecae-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ecae-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4ecae-114">Autenticação de listaMethods</span><span class="sxs-lookup"><span data-stu-id="4ecae-114">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="4ecae-115">[Coleção authenticationMethod](authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="4ecae-115">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="4ecae-116">Leia as propriedades e as relações de todos os objetos **authenticationMethod** de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4ecae-116">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="4ecae-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ecae-117">Properties</span></span>

| <span data-ttu-id="4ecae-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ecae-118">Property</span></span>     | <span data-ttu-id="4ecae-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ecae-119">Type</span></span>        | <span data-ttu-id="4ecae-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ecae-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4ecae-121">id</span><span class="sxs-lookup"><span data-stu-id="4ecae-121">id</span></span>|<span data-ttu-id="4ecae-122">String</span><span class="sxs-lookup"><span data-stu-id="4ecae-122">String</span></span>| <span data-ttu-id="4ecae-123">O identificador dessa instância de um método de autenticação registrado nesse usuário.</span><span class="sxs-lookup"><span data-stu-id="4ecae-123">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="4ecae-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4ecae-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4ecae-125">Relações</span><span class="sxs-lookup"><span data-stu-id="4ecae-125">Relationships</span></span>

<span data-ttu-id="4ecae-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ecae-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ecae-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ecae-127">JSON representation</span></span>

<span data-ttu-id="4ecae-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ecae-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->