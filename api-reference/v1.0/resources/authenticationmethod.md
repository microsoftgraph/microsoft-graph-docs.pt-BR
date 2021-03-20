---
title: tipo de recurso authenticationMethod
description: Representa um método de autenticação registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 283b81981417494e86a225770427f5497490809a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948983"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="05d4e-103">tipo de recurso authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="05d4e-103">authenticationMethod resource type</span></span>

<span data-ttu-id="05d4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05d4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05d4e-105">Representa um método de autenticação registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="05d4e-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="05d4e-106">Um [método de autenticação](/azure/active-directory/authentication/concept-authentication-methods) é algo usado por um usuário para autenticar ou provar sua identidade para o sistema.</span><span class="sxs-lookup"><span data-stu-id="05d4e-106">An [authentication method](/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="05d4e-107">Alguns exemplos incluem senha, telefone (usável por SMS ou chamada de voz), chaves de segurança FIDO2 e muito mais.</span><span class="sxs-lookup"><span data-stu-id="05d4e-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span>

## <a name="methods"></a><span data-ttu-id="05d4e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="05d4e-108">Methods</span></span>

| <span data-ttu-id="05d4e-109">Método</span><span class="sxs-lookup"><span data-stu-id="05d4e-109">Method</span></span>       | <span data-ttu-id="05d4e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="05d4e-110">Return type</span></span> | <span data-ttu-id="05d4e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="05d4e-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="05d4e-112">Autenticação de listaMethods</span><span class="sxs-lookup"><span data-stu-id="05d4e-112">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="05d4e-113">[Coleção authenticationMethod](authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="05d4e-113">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="05d4e-114">Leia as propriedades e as relações de todos os objetos **authenticationMethod** de um usuário.</span><span class="sxs-lookup"><span data-stu-id="05d4e-114">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |
| [<span data-ttu-id="05d4e-115">Obter authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="05d4e-115">Get authenticationMethod</span></span>](../api/authenticationmethod-get.md) | [<span data-ttu-id="05d4e-116">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="05d4e-116">authenticationMethod</span></span>](authenticationmethod.md) | <span data-ttu-id="05d4e-117">Leia as propriedades e as relações de um **objeto authenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="05d4e-117">Read the properties and relationships of an **authenticationMethod** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="05d4e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05d4e-118">Properties</span></span>

| <span data-ttu-id="05d4e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05d4e-119">Property</span></span>     | <span data-ttu-id="05d4e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="05d4e-120">Type</span></span>        | <span data-ttu-id="05d4e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="05d4e-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="05d4e-122">id</span><span class="sxs-lookup"><span data-stu-id="05d4e-122">id</span></span>|<span data-ttu-id="05d4e-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05d4e-123">String</span></span>| <span data-ttu-id="05d4e-124">O identificador dessa instância de um método de autenticação registrado nesse usuário.</span><span class="sxs-lookup"><span data-stu-id="05d4e-124">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="05d4e-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05d4e-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="05d4e-126">Relações</span><span class="sxs-lookup"><span data-stu-id="05d4e-126">Relationships</span></span>

<span data-ttu-id="05d4e-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05d4e-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05d4e-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05d4e-128">JSON representation</span></span>

<span data-ttu-id="05d4e-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05d4e-129">The following is a JSON representation of the resource.</span></span>

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