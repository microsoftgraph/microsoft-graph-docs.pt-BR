---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6151c23bf05b076ade441f908a2810c80f45ed
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253460"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="60736-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="60736-103">managedEBook resource type</span></span>

> <span data-ttu-id="60736-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60736-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60736-105">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="60736-105">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="60736-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="60736-106">Methods</span></span>
|<span data-ttu-id="60736-107">Método</span><span class="sxs-lookup"><span data-stu-id="60736-107">Method</span></span>|<span data-ttu-id="60736-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="60736-108">Return Type</span></span>|<span data-ttu-id="60736-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="60736-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60736-110">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="60736-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="60736-111">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="60736-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="60736-112">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="60736-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="60736-113">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="60736-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="60736-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="60736-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="60736-115">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="60736-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="60736-116">ação assign</span><span class="sxs-lookup"><span data-stu-id="60736-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="60736-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60736-117">None</span></span>|<span data-ttu-id="60736-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="60736-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="60736-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60736-119">Properties</span></span>
|<span data-ttu-id="60736-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60736-120">Property</span></span>|<span data-ttu-id="60736-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="60736-121">Type</span></span>|<span data-ttu-id="60736-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="60736-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60736-123">id</span><span class="sxs-lookup"><span data-stu-id="60736-123">id</span></span>|<span data-ttu-id="60736-124">String</span><span class="sxs-lookup"><span data-stu-id="60736-124">String</span></span>|<span data-ttu-id="60736-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="60736-125">Key of the entity.</span></span>|
|<span data-ttu-id="60736-126">displayName</span><span class="sxs-lookup"><span data-stu-id="60736-126">displayName</span></span>|<span data-ttu-id="60736-127">String</span><span class="sxs-lookup"><span data-stu-id="60736-127">String</span></span>|<span data-ttu-id="60736-128">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="60736-128">Name of the eBook.</span></span>|
|<span data-ttu-id="60736-129">description</span><span class="sxs-lookup"><span data-stu-id="60736-129">description</span></span>|<span data-ttu-id="60736-130">String</span><span class="sxs-lookup"><span data-stu-id="60736-130">String</span></span>|<span data-ttu-id="60736-131">Descrição.</span><span class="sxs-lookup"><span data-stu-id="60736-131">Description.</span></span>|
|<span data-ttu-id="60736-132">publisher</span><span class="sxs-lookup"><span data-stu-id="60736-132">publisher</span></span>|<span data-ttu-id="60736-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60736-133">String</span></span>|<span data-ttu-id="60736-134">Publicador.</span><span class="sxs-lookup"><span data-stu-id="60736-134">Publisher.</span></span>|
|<span data-ttu-id="60736-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="60736-135">publishedDateTime</span></span>|<span data-ttu-id="60736-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60736-136">DateTimeOffset</span></span>|<span data-ttu-id="60736-137">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="60736-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="60736-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="60736-138">largeCover</span></span>|[<span data-ttu-id="60736-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="60736-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="60736-140">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="60736-140">Book cover.</span></span>|
|<span data-ttu-id="60736-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60736-141">createdDateTime</span></span>|<span data-ttu-id="60736-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60736-142">DateTimeOffset</span></span>|<span data-ttu-id="60736-143">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="60736-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="60736-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60736-144">lastModifiedDateTime</span></span>|<span data-ttu-id="60736-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60736-145">DateTimeOffset</span></span>|<span data-ttu-id="60736-146">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="60736-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="60736-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="60736-147">informationUrl</span></span>|<span data-ttu-id="60736-148">String</span><span class="sxs-lookup"><span data-stu-id="60736-148">String</span></span>|<span data-ttu-id="60736-149">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="60736-149">The more information Url.</span></span>|
|<span data-ttu-id="60736-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="60736-150">privacyInformationUrl</span></span>|<span data-ttu-id="60736-151">String</span><span class="sxs-lookup"><span data-stu-id="60736-151">String</span></span>|<span data-ttu-id="60736-152">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="60736-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60736-153">Relações</span><span class="sxs-lookup"><span data-stu-id="60736-153">Relationships</span></span>
|<span data-ttu-id="60736-154">Relação</span><span class="sxs-lookup"><span data-stu-id="60736-154">Relationship</span></span>|<span data-ttu-id="60736-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="60736-155">Type</span></span>|<span data-ttu-id="60736-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="60736-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60736-157">assignments</span><span class="sxs-lookup"><span data-stu-id="60736-157">assignments</span></span>|<span data-ttu-id="60736-158">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="60736-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="60736-159">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="60736-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="60736-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="60736-160">installSummary</span></span>|[<span data-ttu-id="60736-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="60736-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="60736-162">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="60736-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="60736-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="60736-163">deviceStates</span></span>|<span data-ttu-id="60736-164">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="60736-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="60736-165">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="60736-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="60736-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="60736-166">userStateSummary</span></span>|<span data-ttu-id="60736-167">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="60736-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="60736-168">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="60736-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60736-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60736-169">JSON Representation</span></span>
<span data-ttu-id="60736-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60736-170">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



