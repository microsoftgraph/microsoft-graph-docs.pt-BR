---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bf13e2c0a5c8e55a397516c21fe91d65aa413a5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991650"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="2549b-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="2549b-103">managedEBook resource type</span></span>

> <span data-ttu-id="2549b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2549b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2549b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2549b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2549b-106">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="2549b-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="2549b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2549b-107">Methods</span></span>
|<span data-ttu-id="2549b-108">Método</span><span class="sxs-lookup"><span data-stu-id="2549b-108">Method</span></span>|<span data-ttu-id="2549b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2549b-109">Return Type</span></span>|<span data-ttu-id="2549b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2549b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2549b-111">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="2549b-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="2549b-112">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2549b-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="2549b-113">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2549b-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="2549b-114">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="2549b-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="2549b-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="2549b-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="2549b-116">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2549b-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="2549b-117">ação assign</span><span class="sxs-lookup"><span data-stu-id="2549b-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="2549b-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2549b-118">None</span></span>|<span data-ttu-id="2549b-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2549b-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2549b-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2549b-120">Properties</span></span>
|<span data-ttu-id="2549b-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2549b-121">Property</span></span>|<span data-ttu-id="2549b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2549b-122">Type</span></span>|<span data-ttu-id="2549b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2549b-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2549b-124">id</span><span class="sxs-lookup"><span data-stu-id="2549b-124">id</span></span>|<span data-ttu-id="2549b-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2549b-125">String</span></span>|<span data-ttu-id="2549b-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2549b-126">Key of the entity.</span></span>|
|<span data-ttu-id="2549b-127">displayName</span><span class="sxs-lookup"><span data-stu-id="2549b-127">displayName</span></span>|<span data-ttu-id="2549b-128">String</span><span class="sxs-lookup"><span data-stu-id="2549b-128">String</span></span>|<span data-ttu-id="2549b-129">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="2549b-129">Name of the eBook.</span></span>|
|<span data-ttu-id="2549b-130">descrição</span><span class="sxs-lookup"><span data-stu-id="2549b-130">description</span></span>|<span data-ttu-id="2549b-131">String</span><span class="sxs-lookup"><span data-stu-id="2549b-131">String</span></span>|<span data-ttu-id="2549b-132">Descrição.</span><span class="sxs-lookup"><span data-stu-id="2549b-132">Description.</span></span>|
|<span data-ttu-id="2549b-133">publisher</span><span class="sxs-lookup"><span data-stu-id="2549b-133">publisher</span></span>|<span data-ttu-id="2549b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2549b-134">String</span></span>|<span data-ttu-id="2549b-135">Publicador.</span><span class="sxs-lookup"><span data-stu-id="2549b-135">Publisher.</span></span>|
|<span data-ttu-id="2549b-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="2549b-136">publishedDateTime</span></span>|<span data-ttu-id="2549b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2549b-137">DateTimeOffset</span></span>|<span data-ttu-id="2549b-138">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="2549b-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="2549b-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="2549b-139">largeCover</span></span>|[<span data-ttu-id="2549b-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2549b-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2549b-141">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="2549b-141">Book cover.</span></span>|
|<span data-ttu-id="2549b-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2549b-142">createdDateTime</span></span>|<span data-ttu-id="2549b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2549b-143">DateTimeOffset</span></span>|<span data-ttu-id="2549b-144">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2549b-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="2549b-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2549b-145">lastModifiedDateTime</span></span>|<span data-ttu-id="2549b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2549b-146">DateTimeOffset</span></span>|<span data-ttu-id="2549b-147">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="2549b-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="2549b-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2549b-148">informationUrl</span></span>|<span data-ttu-id="2549b-149">String</span><span class="sxs-lookup"><span data-stu-id="2549b-149">String</span></span>|<span data-ttu-id="2549b-150">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2549b-150">The more information Url.</span></span>|
|<span data-ttu-id="2549b-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2549b-151">privacyInformationUrl</span></span>|<span data-ttu-id="2549b-152">String</span><span class="sxs-lookup"><span data-stu-id="2549b-152">String</span></span>|<span data-ttu-id="2549b-153">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2549b-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2549b-154">Relações</span><span class="sxs-lookup"><span data-stu-id="2549b-154">Relationships</span></span>
|<span data-ttu-id="2549b-155">Relação</span><span class="sxs-lookup"><span data-stu-id="2549b-155">Relationship</span></span>|<span data-ttu-id="2549b-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="2549b-156">Type</span></span>|<span data-ttu-id="2549b-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="2549b-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2549b-158">categories</span><span class="sxs-lookup"><span data-stu-id="2549b-158">categories</span></span>|<span data-ttu-id="2549b-159">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2549b-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="2549b-160">A lista de categorias para este eBook.</span><span class="sxs-lookup"><span data-stu-id="2549b-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="2549b-161">assignments</span><span class="sxs-lookup"><span data-stu-id="2549b-161">assignments</span></span>|<span data-ttu-id="2549b-162">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2549b-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="2549b-163">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="2549b-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="2549b-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="2549b-164">installSummary</span></span>|[<span data-ttu-id="2549b-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="2549b-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="2549b-166">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="2549b-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="2549b-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="2549b-167">deviceStates</span></span>|<span data-ttu-id="2549b-168">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="2549b-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="2549b-169">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="2549b-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="2549b-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="2549b-170">userStateSummary</span></span>|<span data-ttu-id="2549b-171">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="2549b-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="2549b-172">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="2549b-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2549b-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2549b-173">JSON Representation</span></span>
<span data-ttu-id="2549b-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2549b-174">Here is a JSON representation of the resource.</span></span>
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





