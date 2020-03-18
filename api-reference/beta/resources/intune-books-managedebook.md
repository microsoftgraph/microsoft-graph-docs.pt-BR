---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcec7c8dfaa0461e6b88d67a5a0f73373a1af7b0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797364"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="e6dc7-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="e6dc7-103">managedEBook resource type</span></span>

> <span data-ttu-id="e6dc7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6dc7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6dc7-106">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="e6dc7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6dc7-107">Methods</span></span>
|<span data-ttu-id="e6dc7-108">Método</span><span class="sxs-lookup"><span data-stu-id="e6dc7-108">Method</span></span>|<span data-ttu-id="e6dc7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6dc7-109">Return Type</span></span>|<span data-ttu-id="e6dc7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6dc7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6dc7-111">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="e6dc7-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="e6dc7-112">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e6dc7-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="e6dc7-113">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e6dc7-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="e6dc7-114">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="e6dc7-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="e6dc7-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="e6dc7-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="e6dc7-116">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e6dc7-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="e6dc7-117">ação assign</span><span class="sxs-lookup"><span data-stu-id="e6dc7-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="e6dc7-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e6dc7-118">None</span></span>|<span data-ttu-id="e6dc7-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e6dc7-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e6dc7-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6dc7-120">Properties</span></span>
|<span data-ttu-id="e6dc7-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6dc7-121">Property</span></span>|<span data-ttu-id="e6dc7-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6dc7-122">Type</span></span>|<span data-ttu-id="e6dc7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6dc7-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6dc7-124">id</span><span class="sxs-lookup"><span data-stu-id="e6dc7-124">id</span></span>|<span data-ttu-id="e6dc7-125">String</span><span class="sxs-lookup"><span data-stu-id="e6dc7-125">String</span></span>|<span data-ttu-id="e6dc7-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-126">Key of the entity.</span></span>|
|<span data-ttu-id="e6dc7-127">displayName</span><span class="sxs-lookup"><span data-stu-id="e6dc7-127">displayName</span></span>|<span data-ttu-id="e6dc7-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dc7-128">String</span></span>|<span data-ttu-id="e6dc7-129">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-129">Name of the eBook.</span></span>|
|<span data-ttu-id="e6dc7-130">description</span><span class="sxs-lookup"><span data-stu-id="e6dc7-130">description</span></span>|<span data-ttu-id="e6dc7-131">String</span><span class="sxs-lookup"><span data-stu-id="e6dc7-131">String</span></span>|<span data-ttu-id="e6dc7-132">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-132">Description.</span></span>|
|<span data-ttu-id="e6dc7-133">publisher</span><span class="sxs-lookup"><span data-stu-id="e6dc7-133">publisher</span></span>|<span data-ttu-id="e6dc7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dc7-134">String</span></span>|<span data-ttu-id="e6dc7-135">Publicador.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-135">Publisher.</span></span>|
|<span data-ttu-id="e6dc7-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6dc7-136">publishedDateTime</span></span>|<span data-ttu-id="e6dc7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6dc7-137">DateTimeOffset</span></span>|<span data-ttu-id="e6dc7-138">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="e6dc7-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="e6dc7-139">largeCover</span></span>|[<span data-ttu-id="e6dc7-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e6dc7-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e6dc7-141">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-141">Book cover.</span></span>|
|<span data-ttu-id="e6dc7-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6dc7-142">createdDateTime</span></span>|<span data-ttu-id="e6dc7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6dc7-143">DateTimeOffset</span></span>|<span data-ttu-id="e6dc7-144">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="e6dc7-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6dc7-145">lastModifiedDateTime</span></span>|<span data-ttu-id="e6dc7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6dc7-146">DateTimeOffset</span></span>|<span data-ttu-id="e6dc7-147">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="e6dc7-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e6dc7-148">informationUrl</span></span>|<span data-ttu-id="e6dc7-149">String</span><span class="sxs-lookup"><span data-stu-id="e6dc7-149">String</span></span>|<span data-ttu-id="e6dc7-150">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-150">The more information Url.</span></span>|
|<span data-ttu-id="e6dc7-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e6dc7-151">privacyInformationUrl</span></span>|<span data-ttu-id="e6dc7-152">String</span><span class="sxs-lookup"><span data-stu-id="e6dc7-152">String</span></span>|<span data-ttu-id="e6dc7-153">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6dc7-154">Relações</span><span class="sxs-lookup"><span data-stu-id="e6dc7-154">Relationships</span></span>
|<span data-ttu-id="e6dc7-155">Relação</span><span class="sxs-lookup"><span data-stu-id="e6dc7-155">Relationship</span></span>|<span data-ttu-id="e6dc7-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6dc7-156">Type</span></span>|<span data-ttu-id="e6dc7-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6dc7-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6dc7-158">categories</span><span class="sxs-lookup"><span data-stu-id="e6dc7-158">categories</span></span>|<span data-ttu-id="e6dc7-159">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="e6dc7-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="e6dc7-160">A lista de categorias para este eBook.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="e6dc7-161">assignments</span><span class="sxs-lookup"><span data-stu-id="e6dc7-161">assignments</span></span>|<span data-ttu-id="e6dc7-162">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e6dc7-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="e6dc7-163">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="e6dc7-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="e6dc7-164">installSummary</span></span>|[<span data-ttu-id="e6dc7-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e6dc7-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="e6dc7-166">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="e6dc7-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="e6dc7-167">deviceStates</span></span>|<span data-ttu-id="e6dc7-168">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="e6dc7-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="e6dc7-169">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="e6dc7-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6dc7-170">userStateSummary</span></span>|<span data-ttu-id="e6dc7-171">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e6dc7-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="e6dc7-172">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6dc7-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6dc7-173">JSON Representation</span></span>
<span data-ttu-id="e6dc7-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6dc7-174">Here is a JSON representation of the resource.</span></span>
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



