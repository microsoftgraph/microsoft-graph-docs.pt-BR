---
title: Tipo de recurso userFlowLanguagePage
description: As páginas de idioma de fluxo de usuário são usadas para determinar as cadeias de caracteres que os usuários serão mostrados durante a jornada do usuário que você configurou usando fluxos de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c76d746aabab06fcc68ffcead238aaf2cc6ddb41
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442712"
---
# <a name="userflowlanguagepage-resource-type"></a><span data-ttu-id="6a3c7-103">Tipo de recurso userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="6a3c7-103">userFlowLanguagePage resource type</span></span>

<span data-ttu-id="6a3c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a3c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a3c7-105">As páginas de idioma de fluxo de usuário são usadas para determinar as cadeias de caracteres que os usuários serão mostrados durante a jornada do usuário que você configurou usando fluxos de usuário.</span><span class="sxs-lookup"><span data-stu-id="6a3c7-105">User flow language pages are used determine the strings users will be shown during the user journey you have configured using user flows.</span></span> <span data-ttu-id="6a3c7-106">Essas páginas de idioma incluem as traduções de idioma padrão fornecidas pela Microsoft ou páginas personalizadas que podem ser criadas para personalizar as traduções de idioma.</span><span class="sxs-lookup"><span data-stu-id="6a3c7-106">These language pages include both the default language translations provided by Microsoft, or custom pages that can be created to customize the language translations.</span></span>

## <a name="methods"></a><span data-ttu-id="6a3c7-107">Methods</span><span class="sxs-lookup"><span data-stu-id="6a3c7-107">Methods</span></span>

|<span data-ttu-id="6a3c7-108">Método</span><span class="sxs-lookup"><span data-stu-id="6a3c7-108">Method</span></span>|<span data-ttu-id="6a3c7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6a3c7-109">Return type</span></span>|<span data-ttu-id="6a3c7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a3c7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a3c7-111">Obter userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="6a3c7-111">Get userFlowLanguagePage</span></span>](../api/userflowlanguagepage-get.md)|[<span data-ttu-id="6a3c7-112">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="6a3c7-112">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="6a3c7-113">Recupere os valores de um objeto [userFlowLanguagePage](../resources/userflowlanguagepage.md) padrão ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="6a3c7-113">Retrieve the values of a default or custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="6a3c7-114">Atualizar userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="6a3c7-114">Update userFlowLanguagePage</span></span>](../api/userflowlanguagepage-put.md)|[<span data-ttu-id="6a3c7-115">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="6a3c7-115">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="6a3c7-116">Atualize os valores em um [objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) personalizado.</span><span class="sxs-lookup"><span data-stu-id="6a3c7-116">Update the values in a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="6a3c7-117">Excluir userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="6a3c7-117">Delete userFlowLanguagePage</span></span>](../api/userflowlanguagepage-delete.md)|<span data-ttu-id="6a3c7-118">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="6a3c7-118">None</span></span>|<span data-ttu-id="6a3c7-119">Exclui os valores de um [objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) personalizado.</span><span class="sxs-lookup"><span data-stu-id="6a3c7-119">Deletes the values from a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a3c7-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a3c7-120">Properties</span></span>

|<span data-ttu-id="6a3c7-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a3c7-121">Property</span></span>|<span data-ttu-id="6a3c7-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a3c7-122">Type</span></span>|<span data-ttu-id="6a3c7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a3c7-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a3c7-124">id</span><span class="sxs-lookup"><span data-stu-id="6a3c7-124">id</span></span>|<span data-ttu-id="6a3c7-125">String</span><span class="sxs-lookup"><span data-stu-id="6a3c7-125">String</span></span>|<span data-ttu-id="6a3c7-126">O identificador da página userFlowLanguage.</span><span class="sxs-lookup"><span data-stu-id="6a3c7-126">The identifier of the userFlowLanguage page.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a3c7-127">Relações</span><span class="sxs-lookup"><span data-stu-id="6a3c7-127">Relationships</span></span>

<span data-ttu-id="6a3c7-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a3c7-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a3c7-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a3c7-129">JSON representation</span></span>

<span data-ttu-id="6a3c7-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a3c7-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguagePage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
