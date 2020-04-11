---
title: tipo de recurso PersonName
description: tipo de recurso PersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e4927ba05443d4b54eaac3f54b7e0d3a8cd62159
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227683"
---
# <a name="personname-resource-type"></a><span data-ttu-id="025ae-103">tipo de recurso PersonName</span><span class="sxs-lookup"><span data-stu-id="025ae-103">personName resource type</span></span>

<span data-ttu-id="025ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="025ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="025ae-105">Representa as informações de nome estendidas fornecidas pelo usuário ou que elas associaram à conta.</span><span class="sxs-lookup"><span data-stu-id="025ae-105">Represents extended name information provided by the user or which they have associated with their account.</span></span>

<span data-ttu-id="025ae-106">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="025ae-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="025ae-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="025ae-107">Methods</span></span>

| <span data-ttu-id="025ae-108">Método</span><span class="sxs-lookup"><span data-stu-id="025ae-108">Method</span></span>                                     | <span data-ttu-id="025ae-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="025ae-109">Return Type</span></span>                 | <span data-ttu-id="025ae-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="025ae-110">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="025ae-111">Obter PersonName</span><span class="sxs-lookup"><span data-stu-id="025ae-111">Get personName</span></span>](../api/personname-get.md) | [<span data-ttu-id="025ae-112">personName</span><span class="sxs-lookup"><span data-stu-id="025ae-112">personName</span></span>](personname.md) | <span data-ttu-id="025ae-113">Leia as propriedades e as relações do objeto PersonName.</span><span class="sxs-lookup"><span data-stu-id="025ae-113">Read properties and relationships of personName object.</span></span> |
| [<span data-ttu-id="025ae-114">Update</span><span class="sxs-lookup"><span data-stu-id="025ae-114">Update</span></span>](../api/personname-update.md)      | [<span data-ttu-id="025ae-115">personName</span><span class="sxs-lookup"><span data-stu-id="025ae-115">personName</span></span>](personname.md) | <span data-ttu-id="025ae-116">Objeto Update PersonName.</span><span class="sxs-lookup"><span data-stu-id="025ae-116">Update personName object.</span></span>                               |
| [<span data-ttu-id="025ae-117">Delete</span><span class="sxs-lookup"><span data-stu-id="025ae-117">Delete</span></span>](../api/personname-delete.md)      | <span data-ttu-id="025ae-118">None</span><span class="sxs-lookup"><span data-stu-id="025ae-118">None</span></span>                        | <span data-ttu-id="025ae-119">Exclua o objeto PersonName.</span><span class="sxs-lookup"><span data-stu-id="025ae-119">Delete personName object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="025ae-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="025ae-120">Properties</span></span>

| <span data-ttu-id="025ae-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="025ae-121">Property</span></span>     | <span data-ttu-id="025ae-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="025ae-122">Type</span></span>                              | <span data-ttu-id="025ae-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="025ae-123">Description</span></span>                                                                                                  |
|:-------------|:----------------------------------|:-------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="025ae-124">displayName</span><span class="sxs-lookup"><span data-stu-id="025ae-124">displayName</span></span>   |<span data-ttu-id="025ae-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="025ae-125">String</span></span>                             | <span data-ttu-id="025ae-126">Fornece uma renderização ordenada de firstName e lastName, dependendo da localidade do usuário ou de seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="025ae-126">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span> |
|<span data-ttu-id="025ae-127">primeiro</span><span class="sxs-lookup"><span data-stu-id="025ae-127">first</span></span>         |<span data-ttu-id="025ae-128">String</span><span class="sxs-lookup"><span data-stu-id="025ae-128">String</span></span>                             | <span data-ttu-id="025ae-129">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="025ae-129">First Name of the user.</span></span>                                                                                      |
|<span data-ttu-id="025ae-130">initials</span><span class="sxs-lookup"><span data-stu-id="025ae-130">initials</span></span>      |<span data-ttu-id="025ae-131">String</span><span class="sxs-lookup"><span data-stu-id="025ae-131">String</span></span>                             | <span data-ttu-id="025ae-132">Iniciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="025ae-132">Initials of the user.</span></span>                                                                                        |
|<span data-ttu-id="025ae-133">languageTag</span><span class="sxs-lookup"><span data-stu-id="025ae-133">languageTag</span></span>   |<span data-ttu-id="025ae-134">String</span><span class="sxs-lookup"><span data-stu-id="025ae-134">String</span></span>                             | <span data-ttu-id="025ae-135">Contém o nome do idioma (en-US, no-NB, en-AU) após o formato BCP47 da IETF.</span><span class="sxs-lookup"><span data-stu-id="025ae-135">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>                        |
|<span data-ttu-id="025ae-136">durar</span><span class="sxs-lookup"><span data-stu-id="025ae-136">last</span></span>          |<span data-ttu-id="025ae-137">String</span><span class="sxs-lookup"><span data-stu-id="025ae-137">String</span></span>                             | <span data-ttu-id="025ae-138">Sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="025ae-138">Last Name of the user.</span></span>                                                                                       |
|<span data-ttu-id="025ae-139">Virgem</span><span class="sxs-lookup"><span data-stu-id="025ae-139">maiden</span></span>        |<span data-ttu-id="025ae-140">String</span><span class="sxs-lookup"><span data-stu-id="025ae-140">String</span></span>                             | <span data-ttu-id="025ae-141">Nome de solteira do usuário.</span><span class="sxs-lookup"><span data-stu-id="025ae-141">Maiden Name of the user.</span></span>                                                                                     |
|<span data-ttu-id="025ae-142">middleware</span><span class="sxs-lookup"><span data-stu-id="025ae-142">middle</span></span>        |<span data-ttu-id="025ae-143">String</span><span class="sxs-lookup"><span data-stu-id="025ae-143">String</span></span>                             | <span data-ttu-id="025ae-144">Middlie nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="025ae-144">Middlie Name of the user.</span></span>                                                                                    |
|<span data-ttu-id="025ae-145">apelido</span><span class="sxs-lookup"><span data-stu-id="025ae-145">nickname</span></span>      |<span data-ttu-id="025ae-146">String</span><span class="sxs-lookup"><span data-stu-id="025ae-146">String</span></span>                             | <span data-ttu-id="025ae-147">Apelido do usuário.</span><span class="sxs-lookup"><span data-stu-id="025ae-147">Nickname of the user.</span></span>                                                                                        |
|<span data-ttu-id="025ae-148">pronúncia</span><span class="sxs-lookup"><span data-stu-id="025ae-148">pronunciation</span></span> |[<span data-ttu-id="025ae-149">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="025ae-149">yomiPersonName</span></span>](yomipersonname.md)| <span data-ttu-id="025ae-150">Orientações sobre como pronunciar o nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="025ae-150">Guidance on how to pronounce the users name.</span></span>                                                                 |
|<span data-ttu-id="025ae-151">sufixo</span><span class="sxs-lookup"><span data-stu-id="025ae-151">suffix</span></span>        |<span data-ttu-id="025ae-152">String</span><span class="sxs-lookup"><span data-stu-id="025ae-152">String</span></span>                             | <span data-ttu-id="025ae-153">Designadores usados após o nome dos usuários (por exemplo: PhD).</span><span class="sxs-lookup"><span data-stu-id="025ae-153">Designators used after the users name (eg: PhD.)</span></span>                                                             |
|<span data-ttu-id="025ae-154">title</span><span class="sxs-lookup"><span data-stu-id="025ae-154">title</span></span>         |<span data-ttu-id="025ae-155">String</span><span class="sxs-lookup"><span data-stu-id="025ae-155">String</span></span>                             | <span data-ttu-id="025ae-156">Honorifics usado para prefixar um nome de usuário (por exemplo: Dr, Sir, Madam, Sra.)</span><span class="sxs-lookup"><span data-stu-id="025ae-156">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="025ae-157">Relações</span><span class="sxs-lookup"><span data-stu-id="025ae-157">Relationships</span></span>

<span data-ttu-id="025ae-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="025ae-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="025ae-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="025ae-159">JSON representation</span></span>

<span data-ttu-id="025ae-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="025ae-160">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personName",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "initials": "String",
  "languageTag": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String",
  "nickname": "String",
  "pronunciation": {"@odata.type": "microsoft.graph.yomiPersonName"},
  "suffix": "String",
  "title": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->