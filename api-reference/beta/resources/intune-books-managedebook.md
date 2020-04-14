---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f3bcbd777c87150103fe21495370adddf3afe90
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403011"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="c3fb1-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="c3fb1-103">managedEBook resource type</span></span>

<span data-ttu-id="c3fb1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3fb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3fb1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3fb1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3fb1-107">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="c3fb1-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c3fb1-108">Methods</span></span>
|<span data-ttu-id="c3fb1-109">Método</span><span class="sxs-lookup"><span data-stu-id="c3fb1-109">Method</span></span>|<span data-ttu-id="c3fb1-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c3fb1-110">Return Type</span></span>|<span data-ttu-id="c3fb1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3fb1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3fb1-112">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="c3fb1-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="c3fb1-113">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="c3fb1-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="c3fb1-114">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c3fb1-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="c3fb1-115">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="c3fb1-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="c3fb1-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="c3fb1-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="c3fb1-117">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c3fb1-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="c3fb1-118">ação assign</span><span class="sxs-lookup"><span data-stu-id="c3fb1-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="c3fb1-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c3fb1-119">None</span></span>|<span data-ttu-id="c3fb1-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c3fb1-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c3fb1-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3fb1-121">Properties</span></span>
|<span data-ttu-id="c3fb1-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3fb1-122">Property</span></span>|<span data-ttu-id="c3fb1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3fb1-123">Type</span></span>|<span data-ttu-id="c3fb1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3fb1-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3fb1-125">id</span><span class="sxs-lookup"><span data-stu-id="c3fb1-125">id</span></span>|<span data-ttu-id="c3fb1-126">String</span><span class="sxs-lookup"><span data-stu-id="c3fb1-126">String</span></span>|<span data-ttu-id="c3fb1-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-127">Key of the entity.</span></span>|
|<span data-ttu-id="c3fb1-128">displayName</span><span class="sxs-lookup"><span data-stu-id="c3fb1-128">displayName</span></span>|<span data-ttu-id="c3fb1-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3fb1-129">String</span></span>|<span data-ttu-id="c3fb1-130">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-130">Name of the eBook.</span></span>|
|<span data-ttu-id="c3fb1-131">description</span><span class="sxs-lookup"><span data-stu-id="c3fb1-131">description</span></span>|<span data-ttu-id="c3fb1-132">String</span><span class="sxs-lookup"><span data-stu-id="c3fb1-132">String</span></span>|<span data-ttu-id="c3fb1-133">Descrição.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-133">Description.</span></span>|
|<span data-ttu-id="c3fb1-134">publisher</span><span class="sxs-lookup"><span data-stu-id="c3fb1-134">publisher</span></span>|<span data-ttu-id="c3fb1-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3fb1-135">String</span></span>|<span data-ttu-id="c3fb1-136">Publicador.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-136">Publisher.</span></span>|
|<span data-ttu-id="c3fb1-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3fb1-137">publishedDateTime</span></span>|<span data-ttu-id="c3fb1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3fb1-138">DateTimeOffset</span></span>|<span data-ttu-id="c3fb1-139">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="c3fb1-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="c3fb1-140">largeCover</span></span>|[<span data-ttu-id="c3fb1-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c3fb1-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c3fb1-142">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-142">Book cover.</span></span>|
|<span data-ttu-id="c3fb1-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3fb1-143">createdDateTime</span></span>|<span data-ttu-id="c3fb1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3fb1-144">DateTimeOffset</span></span>|<span data-ttu-id="c3fb1-145">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="c3fb1-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3fb1-146">lastModifiedDateTime</span></span>|<span data-ttu-id="c3fb1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3fb1-147">DateTimeOffset</span></span>|<span data-ttu-id="c3fb1-148">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="c3fb1-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c3fb1-149">informationUrl</span></span>|<span data-ttu-id="c3fb1-150">String</span><span class="sxs-lookup"><span data-stu-id="c3fb1-150">String</span></span>|<span data-ttu-id="c3fb1-151">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-151">The more information Url.</span></span>|
|<span data-ttu-id="c3fb1-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c3fb1-152">privacyInformationUrl</span></span>|<span data-ttu-id="c3fb1-153">String</span><span class="sxs-lookup"><span data-stu-id="c3fb1-153">String</span></span>|<span data-ttu-id="c3fb1-154">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3fb1-155">Relações</span><span class="sxs-lookup"><span data-stu-id="c3fb1-155">Relationships</span></span>
|<span data-ttu-id="c3fb1-156">Relação</span><span class="sxs-lookup"><span data-stu-id="c3fb1-156">Relationship</span></span>|<span data-ttu-id="c3fb1-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3fb1-157">Type</span></span>|<span data-ttu-id="c3fb1-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3fb1-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3fb1-159">categories</span><span class="sxs-lookup"><span data-stu-id="c3fb1-159">categories</span></span>|<span data-ttu-id="c3fb1-160">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="c3fb1-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="c3fb1-161">A lista de categorias para este eBook.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="c3fb1-162">assignments</span><span class="sxs-lookup"><span data-stu-id="c3fb1-162">assignments</span></span>|<span data-ttu-id="c3fb1-163">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c3fb1-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="c3fb1-164">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="c3fb1-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="c3fb1-165">installSummary</span></span>|[<span data-ttu-id="c3fb1-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c3fb1-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="c3fb1-167">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="c3fb1-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="c3fb1-168">deviceStates</span></span>|<span data-ttu-id="c3fb1-169">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="c3fb1-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="c3fb1-170">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="c3fb1-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="c3fb1-171">userStateSummary</span></span>|<span data-ttu-id="c3fb1-172">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="c3fb1-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="c3fb1-173">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3fb1-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3fb1-174">JSON Representation</span></span>
<span data-ttu-id="c3fb1-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3fb1-175">Here is a JSON representation of the resource.</span></span>
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



