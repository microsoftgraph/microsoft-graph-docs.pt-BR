---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a9248a2bca56188deb913159d9ff664ce8d9b48
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949294"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="5a5b5-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="5a5b5-103">managedEBook resource type</span></span>

> <span data-ttu-id="5a5b5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a5b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a5b5-106">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="5a5b5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5a5b5-107">Methods</span></span>
|<span data-ttu-id="5a5b5-108">Método</span><span class="sxs-lookup"><span data-stu-id="5a5b5-108">Method</span></span>|<span data-ttu-id="5a5b5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5a5b5-109">Return Type</span></span>|<span data-ttu-id="5a5b5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a5b5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a5b5-111">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="5a5b5-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="5a5b5-112">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="5a5b5-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="5a5b5-113">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5a5b5-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="5a5b5-114">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="5a5b5-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="5a5b5-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="5a5b5-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="5a5b5-116">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5a5b5-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="5a5b5-117">ação assign</span><span class="sxs-lookup"><span data-stu-id="5a5b5-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="5a5b5-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5a5b5-118">None</span></span>|<span data-ttu-id="5a5b5-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5a5b5-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5a5b5-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a5b5-120">Properties</span></span>
|<span data-ttu-id="5a5b5-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a5b5-121">Property</span></span>|<span data-ttu-id="5a5b5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a5b5-122">Type</span></span>|<span data-ttu-id="5a5b5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a5b5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a5b5-124">id</span><span class="sxs-lookup"><span data-stu-id="5a5b5-124">id</span></span>|<span data-ttu-id="5a5b5-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a5b5-125">String</span></span>|<span data-ttu-id="5a5b5-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-126">Key of the entity.</span></span>|
|<span data-ttu-id="5a5b5-127">displayName</span><span class="sxs-lookup"><span data-stu-id="5a5b5-127">displayName</span></span>|<span data-ttu-id="5a5b5-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a5b5-128">String</span></span>|<span data-ttu-id="5a5b5-129">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-129">Name of the eBook.</span></span>|
|<span data-ttu-id="5a5b5-130">description</span><span class="sxs-lookup"><span data-stu-id="5a5b5-130">description</span></span>|<span data-ttu-id="5a5b5-131">String</span><span class="sxs-lookup"><span data-stu-id="5a5b5-131">String</span></span>|<span data-ttu-id="5a5b5-132">Descrição.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-132">Description.</span></span>|
|<span data-ttu-id="5a5b5-133">publisher</span><span class="sxs-lookup"><span data-stu-id="5a5b5-133">publisher</span></span>|<span data-ttu-id="5a5b5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a5b5-134">String</span></span>|<span data-ttu-id="5a5b5-135">Publicador.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-135">Publisher.</span></span>|
|<span data-ttu-id="5a5b5-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a5b5-136">publishedDateTime</span></span>|<span data-ttu-id="5a5b5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a5b5-137">DateTimeOffset</span></span>|<span data-ttu-id="5a5b5-138">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="5a5b5-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="5a5b5-139">largeCover</span></span>|[<span data-ttu-id="5a5b5-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5a5b5-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5a5b5-141">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-141">Book cover.</span></span>|
|<span data-ttu-id="5a5b5-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a5b5-142">createdDateTime</span></span>|<span data-ttu-id="5a5b5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a5b5-143">DateTimeOffset</span></span>|<span data-ttu-id="5a5b5-144">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="5a5b5-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a5b5-145">lastModifiedDateTime</span></span>|<span data-ttu-id="5a5b5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a5b5-146">DateTimeOffset</span></span>|<span data-ttu-id="5a5b5-147">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="5a5b5-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5a5b5-148">informationUrl</span></span>|<span data-ttu-id="5a5b5-149">String</span><span class="sxs-lookup"><span data-stu-id="5a5b5-149">String</span></span>|<span data-ttu-id="5a5b5-150">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-150">The more information Url.</span></span>|
|<span data-ttu-id="5a5b5-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5a5b5-151">privacyInformationUrl</span></span>|<span data-ttu-id="5a5b5-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a5b5-152">String</span></span>|<span data-ttu-id="5a5b5-153">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a5b5-154">Relações</span><span class="sxs-lookup"><span data-stu-id="5a5b5-154">Relationships</span></span>
|<span data-ttu-id="5a5b5-155">Relação</span><span class="sxs-lookup"><span data-stu-id="5a5b5-155">Relationship</span></span>|<span data-ttu-id="5a5b5-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a5b5-156">Type</span></span>|<span data-ttu-id="5a5b5-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a5b5-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a5b5-158">categories</span><span class="sxs-lookup"><span data-stu-id="5a5b5-158">categories</span></span>|<span data-ttu-id="5a5b5-159">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="5a5b5-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="5a5b5-160">A lista de categorias para este eBook.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="5a5b5-161">assignments</span><span class="sxs-lookup"><span data-stu-id="5a5b5-161">assignments</span></span>|<span data-ttu-id="5a5b5-162">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5a5b5-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="5a5b5-163">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="5a5b5-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="5a5b5-164">installSummary</span></span>|[<span data-ttu-id="5a5b5-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5a5b5-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5a5b5-166">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="5a5b5-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="5a5b5-167">deviceStates</span></span>|<span data-ttu-id="5a5b5-168">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="5a5b5-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="5a5b5-169">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="5a5b5-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="5a5b5-170">userStateSummary</span></span>|<span data-ttu-id="5a5b5-171">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="5a5b5-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="5a5b5-172">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a5b5-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a5b5-173">JSON Representation</span></span>
<span data-ttu-id="5a5b5-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a5b5-174">Here is a JSON representation of the resource.</span></span>
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




