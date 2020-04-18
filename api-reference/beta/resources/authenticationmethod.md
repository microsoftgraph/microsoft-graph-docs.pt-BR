---
title: tipo de recurso authenticationMethod
description: Representa um método de autenticação registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fefa2ed8ee17a898b51e7bc21b3e13ec64f68d56
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557833"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="c388e-103">tipo de recurso authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c388e-103">authenticationMethod resource type</span></span>

<span data-ttu-id="c388e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c388e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c388e-105">Representa um método de autenticação registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="c388e-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="c388e-106">Um [método de autenticação](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) é algo usado por um usuário para autenticar ou provar sua identidade para o sistema.</span><span class="sxs-lookup"><span data-stu-id="c388e-106">An [authentication method](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="c388e-107">Alguns exemplos incluem senha, telefone (utilizável via SMS ou chamada de voz), chaves de segurança do FIDO2 e muito mais.</span><span class="sxs-lookup"><span data-stu-id="c388e-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span> <span data-ttu-id="c388e-108">No momento, os métodos Password e Phone são implementados.</span><span class="sxs-lookup"><span data-stu-id="c388e-108">Currently, password and phone methods are implemented.</span></span>

## <a name="methods"></a><span data-ttu-id="c388e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="c388e-109">Methods</span></span>

| <span data-ttu-id="c388e-110">Método</span><span class="sxs-lookup"><span data-stu-id="c388e-110">Method</span></span>       | <span data-ttu-id="c388e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c388e-111">Return type</span></span> | <span data-ttu-id="c388e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c388e-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c388e-113">Listar authenticationMethods</span><span class="sxs-lookup"><span data-stu-id="c388e-113">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="c388e-114">coleção [AuthenticationMethod](authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="c388e-114">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="c388e-115">Leia as propriedades e os relacionamentos de todos os objetos do usuário **AuthenticationMethod** .</span><span class="sxs-lookup"><span data-stu-id="c388e-115">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |
| [<span data-ttu-id="c388e-116">Obter authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c388e-116">Get authenticationMethod</span></span>](../api/authenticationmethod-get.md) | [<span data-ttu-id="c388e-117">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c388e-117">authenticationMethod</span></span>](authenticationmethod.md) | <span data-ttu-id="c388e-118">Leia as propriedades e os relacionamentos de um objeto **AuthenticationMethod** .</span><span class="sxs-lookup"><span data-stu-id="c388e-118">Read the properties and relationships of an **authenticationMethod** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c388e-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c388e-119">Properties</span></span>

| <span data-ttu-id="c388e-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c388e-120">Property</span></span>     | <span data-ttu-id="c388e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c388e-121">Type</span></span>        | <span data-ttu-id="c388e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c388e-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c388e-123">id</span><span class="sxs-lookup"><span data-stu-id="c388e-123">id</span></span>|<span data-ttu-id="c388e-124">String</span><span class="sxs-lookup"><span data-stu-id="c388e-124">String</span></span>| <span data-ttu-id="c388e-125">O identificador da instância de um método de autenticação registrado para este usuário.</span><span class="sxs-lookup"><span data-stu-id="c388e-125">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="c388e-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c388e-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c388e-127">Relações</span><span class="sxs-lookup"><span data-stu-id="c388e-127">Relationships</span></span>

<span data-ttu-id="c388e-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c388e-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c388e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c388e-129">JSON representation</span></span>

<span data-ttu-id="c388e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c388e-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
  "baseType": "",
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
