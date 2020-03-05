---
title: tipo de recurso webaccount
description: tipo de recurso webaccount
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ceb282dbcf0370e5eca2001b582660bdcaa1f1aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519446"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="cc1dc-103">tipo de recurso webaccount</span><span class="sxs-lookup"><span data-stu-id="cc1dc-103">webAccount resource type</span></span>

<span data-ttu-id="cc1dc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cc1dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc1dc-105">Representa contas da Web que o usuário indicou que usa ou adicionou ao [perfil](profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="cc1dc-105">Represents web accounts the user has indicated they use or has added to their user [profile](profile.md).</span></span>

<span data-ttu-id="cc1dc-106">Esse tipo de recurso herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cc1dc-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cc1dc-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cc1dc-107">Methods</span></span>

| <span data-ttu-id="cc1dc-108">Método</span><span class="sxs-lookup"><span data-stu-id="cc1dc-108">Method</span></span>                                     | <span data-ttu-id="cc1dc-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cc1dc-109">Return Type</span></span>                 | <span data-ttu-id="cc1dc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc1dc-110">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="cc1dc-111">Obter webaccount</span><span class="sxs-lookup"><span data-stu-id="cc1dc-111">Get webAccount</span></span>](../api/webaccount-get.md) | [<span data-ttu-id="cc1dc-112">conta da</span><span class="sxs-lookup"><span data-stu-id="cc1dc-112">webAccount</span></span>](webaccount.md) | <span data-ttu-id="cc1dc-113">Leia as propriedades e os relacionamentos de um objeto **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="cc1dc-113">Read the properties and relationships of a **webAccount** object.</span></span> |
| [<span data-ttu-id="cc1dc-114">Atualizar webaccount</span><span class="sxs-lookup"><span data-stu-id="cc1dc-114">Update webAccount</span></span>](../api/webaccount-update.md)      | [<span data-ttu-id="cc1dc-115">conta da</span><span class="sxs-lookup"><span data-stu-id="cc1dc-115">webAccount</span></span>](webaccount.md) | <span data-ttu-id="cc1dc-116">Atualize um objeto **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="cc1dc-116">Update a **webAccount** object.</span></span>                               |
| [<span data-ttu-id="cc1dc-117">Excluir conta da</span><span class="sxs-lookup"><span data-stu-id="cc1dc-117">Delete webAccount</span></span>](../api/webaccount-delete.md)      | <span data-ttu-id="cc1dc-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc1dc-118">None</span></span>                        | <span data-ttu-id="cc1dc-119">Excluir um objeto **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="cc1dc-119">Delete a **webAccount** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="cc1dc-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc1dc-120">Properties</span></span>

| <span data-ttu-id="cc1dc-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc1dc-121">Property</span></span>     | <span data-ttu-id="cc1dc-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc1dc-122">Type</span></span>                                      | <span data-ttu-id="cc1dc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc1dc-123">Description</span></span>                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="cc1dc-124">description</span><span class="sxs-lookup"><span data-stu-id="cc1dc-124">description</span></span>   |<span data-ttu-id="cc1dc-125">String</span><span class="sxs-lookup"><span data-stu-id="cc1dc-125">String</span></span>                                     | <span data-ttu-id="cc1dc-126">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="cc1dc-126">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="cc1dc-127">service</span><span class="sxs-lookup"><span data-stu-id="cc1dc-127">service</span></span>       |[<span data-ttu-id="cc1dc-128">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="cc1dc-128">serviceInformation</span></span>](serviceinformation.md)| <span data-ttu-id="cc1dc-129">Contém detalhes básicos sobre o serviço que está sendo associado.</span><span class="sxs-lookup"><span data-stu-id="cc1dc-129">Contains basic detail about the service that is being associated.</span></span>                              |
|<span data-ttu-id="cc1dc-130">statusMessage</span><span class="sxs-lookup"><span data-stu-id="cc1dc-130">statusMessage</span></span> |<span data-ttu-id="cc1dc-131">String</span><span class="sxs-lookup"><span data-stu-id="cc1dc-131">String</span></span>                                     | <span data-ttu-id="cc1dc-132">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="cc1dc-132">Contains a status message from the cloud service if provided or synchronized.</span></span>                  |
|<span data-ttu-id="cc1dc-133">userId</span><span class="sxs-lookup"><span data-stu-id="cc1dc-133">userId</span></span>        |<span data-ttu-id="cc1dc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc1dc-134">String</span></span>                                     | <span data-ttu-id="cc1dc-135">O nome de usuário exibido para a conta da Web.</span><span class="sxs-lookup"><span data-stu-id="cc1dc-135">The user name  displayed for the webaccount.</span></span>                                    |
|<span data-ttu-id="cc1dc-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="cc1dc-136">webUrl</span></span>        |<span data-ttu-id="cc1dc-137">String</span><span class="sxs-lookup"><span data-stu-id="cc1dc-137">String</span></span>                                     | <span data-ttu-id="cc1dc-138">Contém um link para o perfil do usuário no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="cc1dc-138">Contains a link to the user's profile on the cloud service if one exists.</span></span>                       |

## <a name="relationships"></a><span data-ttu-id="cc1dc-139">Relações</span><span class="sxs-lookup"><span data-stu-id="cc1dc-139">Relationships</span></span>

<span data-ttu-id="cc1dc-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc1dc-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc1dc-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc1dc-141">JSON representation</span></span>

<span data-ttu-id="cc1dc-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc1dc-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": ""
}-->

```json
{
  "description": "String",
  "service": {"@odata.type": "microsoft.graph.serviceInformation"},
  "statusMessage": "String",
  "userId": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webAccount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
