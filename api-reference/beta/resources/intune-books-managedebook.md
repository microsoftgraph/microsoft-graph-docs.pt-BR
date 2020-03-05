---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 040da9c471d42ff77423dc035cce8b255ab9299a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488723"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="c9293-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="c9293-103">managedEBook resource type</span></span>

<span data-ttu-id="c9293-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c9293-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9293-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9293-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9293-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9293-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9293-107">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="c9293-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="c9293-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c9293-108">Methods</span></span>
|<span data-ttu-id="c9293-109">Método</span><span class="sxs-lookup"><span data-stu-id="c9293-109">Method</span></span>|<span data-ttu-id="c9293-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c9293-110">Return Type</span></span>|<span data-ttu-id="c9293-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9293-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c9293-112">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="c9293-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="c9293-113">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="c9293-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="c9293-114">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c9293-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="c9293-115">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="c9293-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="c9293-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="c9293-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="c9293-117">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c9293-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="c9293-118">ação assign</span><span class="sxs-lookup"><span data-stu-id="c9293-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="c9293-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c9293-119">None</span></span>|<span data-ttu-id="c9293-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c9293-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c9293-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9293-121">Properties</span></span>
|<span data-ttu-id="c9293-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9293-122">Property</span></span>|<span data-ttu-id="c9293-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9293-123">Type</span></span>|<span data-ttu-id="c9293-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9293-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9293-125">id</span><span class="sxs-lookup"><span data-stu-id="c9293-125">id</span></span>|<span data-ttu-id="c9293-126">String</span><span class="sxs-lookup"><span data-stu-id="c9293-126">String</span></span>|<span data-ttu-id="c9293-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c9293-127">Key of the entity.</span></span>|
|<span data-ttu-id="c9293-128">displayName</span><span class="sxs-lookup"><span data-stu-id="c9293-128">displayName</span></span>|<span data-ttu-id="c9293-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9293-129">String</span></span>|<span data-ttu-id="c9293-130">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c9293-130">Name of the eBook.</span></span>|
|<span data-ttu-id="c9293-131">description</span><span class="sxs-lookup"><span data-stu-id="c9293-131">description</span></span>|<span data-ttu-id="c9293-132">String</span><span class="sxs-lookup"><span data-stu-id="c9293-132">String</span></span>|<span data-ttu-id="c9293-133">Descrição.</span><span class="sxs-lookup"><span data-stu-id="c9293-133">Description.</span></span>|
|<span data-ttu-id="c9293-134">publisher</span><span class="sxs-lookup"><span data-stu-id="c9293-134">publisher</span></span>|<span data-ttu-id="c9293-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9293-135">String</span></span>|<span data-ttu-id="c9293-136">Publicador.</span><span class="sxs-lookup"><span data-stu-id="c9293-136">Publisher.</span></span>|
|<span data-ttu-id="c9293-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9293-137">publishedDateTime</span></span>|<span data-ttu-id="c9293-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9293-138">DateTimeOffset</span></span>|<span data-ttu-id="c9293-139">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="c9293-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="c9293-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="c9293-140">largeCover</span></span>|[<span data-ttu-id="c9293-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c9293-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c9293-142">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="c9293-142">Book cover.</span></span>|
|<span data-ttu-id="c9293-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9293-143">createdDateTime</span></span>|<span data-ttu-id="c9293-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9293-144">DateTimeOffset</span></span>|<span data-ttu-id="c9293-145">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c9293-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="c9293-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9293-146">lastModifiedDateTime</span></span>|<span data-ttu-id="c9293-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9293-147">DateTimeOffset</span></span>|<span data-ttu-id="c9293-148">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c9293-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="c9293-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c9293-149">informationUrl</span></span>|<span data-ttu-id="c9293-150">String</span><span class="sxs-lookup"><span data-stu-id="c9293-150">String</span></span>|<span data-ttu-id="c9293-151">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c9293-151">The more information Url.</span></span>|
|<span data-ttu-id="c9293-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c9293-152">privacyInformationUrl</span></span>|<span data-ttu-id="c9293-153">String</span><span class="sxs-lookup"><span data-stu-id="c9293-153">String</span></span>|<span data-ttu-id="c9293-154">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c9293-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9293-155">Relações</span><span class="sxs-lookup"><span data-stu-id="c9293-155">Relationships</span></span>
|<span data-ttu-id="c9293-156">Relação</span><span class="sxs-lookup"><span data-stu-id="c9293-156">Relationship</span></span>|<span data-ttu-id="c9293-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9293-157">Type</span></span>|<span data-ttu-id="c9293-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9293-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9293-159">categories</span><span class="sxs-lookup"><span data-stu-id="c9293-159">categories</span></span>|<span data-ttu-id="c9293-160">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="c9293-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="c9293-161">A lista de categorias para este eBook.</span><span class="sxs-lookup"><span data-stu-id="c9293-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="c9293-162">assignments</span><span class="sxs-lookup"><span data-stu-id="c9293-162">assignments</span></span>|<span data-ttu-id="c9293-163">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c9293-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="c9293-164">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c9293-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="c9293-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="c9293-165">installSummary</span></span>|[<span data-ttu-id="c9293-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c9293-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="c9293-167">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c9293-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="c9293-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="c9293-168">deviceStates</span></span>|<span data-ttu-id="c9293-169">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="c9293-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="c9293-170">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c9293-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="c9293-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="c9293-171">userStateSummary</span></span>|<span data-ttu-id="c9293-172">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="c9293-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="c9293-173">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c9293-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9293-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9293-174">JSON Representation</span></span>
<span data-ttu-id="c9293-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9293-175">Here is a JSON representation of the resource.</span></span>
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



