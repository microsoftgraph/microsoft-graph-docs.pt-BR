---
title: tipo de recurso authenticationMethod
description: Representa um método de autenticação registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b9510a53ea80142bd9f155dce3e12824ad2d186e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034119"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="59088-103">tipo de recurso authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="59088-103">authenticationMethod resource type</span></span>

<span data-ttu-id="59088-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59088-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59088-105">Representa um método de autenticação registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="59088-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="59088-106">Um [método de autenticação](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) é algo usado por um usuário para autenticar ou provar sua identidade para o sistema.</span><span class="sxs-lookup"><span data-stu-id="59088-106">An [authentication method](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="59088-107">Alguns exemplos incluem senha, telefone (utilizável via SMS ou chamada de voz), chaves de segurança do FIDO2 e muito mais.</span><span class="sxs-lookup"><span data-stu-id="59088-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span> <span data-ttu-id="59088-108">No momento, os métodos Password e Phone são implementados.</span><span class="sxs-lookup"><span data-stu-id="59088-108">Currently, password and phone methods are implemented.</span></span>

## <a name="methods"></a><span data-ttu-id="59088-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="59088-109">Methods</span></span>

| <span data-ttu-id="59088-110">Método</span><span class="sxs-lookup"><span data-stu-id="59088-110">Method</span></span>       | <span data-ttu-id="59088-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="59088-111">Return type</span></span> | <span data-ttu-id="59088-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="59088-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="59088-113">Listar authenticationMethods</span><span class="sxs-lookup"><span data-stu-id="59088-113">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="59088-114">coleção [AuthenticationMethod](authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="59088-114">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="59088-115">Leia as propriedades e os relacionamentos de todos os objetos do usuário **AuthenticationMethod** .</span><span class="sxs-lookup"><span data-stu-id="59088-115">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |
| [<span data-ttu-id="59088-116">Obter authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="59088-116">Get authenticationMethod</span></span>](../api/authenticationmethod-get.md) | [<span data-ttu-id="59088-117">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="59088-117">authenticationMethod</span></span>](authenticationmethod.md) | <span data-ttu-id="59088-118">Leia as propriedades e os relacionamentos de um objeto **AuthenticationMethod** .</span><span class="sxs-lookup"><span data-stu-id="59088-118">Read the properties and relationships of an **authenticationMethod** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="59088-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59088-119">Properties</span></span>

| <span data-ttu-id="59088-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59088-120">Property</span></span>     | <span data-ttu-id="59088-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="59088-121">Type</span></span>        | <span data-ttu-id="59088-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="59088-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59088-123">id</span><span class="sxs-lookup"><span data-stu-id="59088-123">id</span></span>|<span data-ttu-id="59088-124">String</span><span class="sxs-lookup"><span data-stu-id="59088-124">String</span></span>| <span data-ttu-id="59088-125">O identificador da instância de um método de autenticação registrado para este usuário.</span><span class="sxs-lookup"><span data-stu-id="59088-125">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="59088-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59088-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="59088-127">Relações</span><span class="sxs-lookup"><span data-stu-id="59088-127">Relationships</span></span>

<span data-ttu-id="59088-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59088-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59088-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59088-129">JSON representation</span></span>

<span data-ttu-id="59088-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59088-130">The following is a JSON representation of the resource.</span></span>

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


