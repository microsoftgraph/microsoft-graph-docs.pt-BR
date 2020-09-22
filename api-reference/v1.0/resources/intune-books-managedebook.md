---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ee5bb486346e315ae00b0e54f44a9fd9b7613c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088668"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="c54b3-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="c54b3-103">managedEBook resource type</span></span>

<span data-ttu-id="c54b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c54b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c54b3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c54b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c54b3-106">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="c54b3-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="c54b3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c54b3-107">Methods</span></span>
|<span data-ttu-id="c54b3-108">Método</span><span class="sxs-lookup"><span data-stu-id="c54b3-108">Method</span></span>|<span data-ttu-id="c54b3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c54b3-109">Return Type</span></span>|<span data-ttu-id="c54b3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54b3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c54b3-111">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="c54b3-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="c54b3-112">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="c54b3-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="c54b3-113">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c54b3-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="c54b3-114">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="c54b3-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="c54b3-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="c54b3-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="c54b3-116">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c54b3-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="c54b3-117">ação assign</span><span class="sxs-lookup"><span data-stu-id="c54b3-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="c54b3-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c54b3-118">None</span></span>|<span data-ttu-id="c54b3-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c54b3-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c54b3-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c54b3-120">Properties</span></span>
|<span data-ttu-id="c54b3-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c54b3-121">Property</span></span>|<span data-ttu-id="c54b3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c54b3-122">Type</span></span>|<span data-ttu-id="c54b3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54b3-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c54b3-124">id</span><span class="sxs-lookup"><span data-stu-id="c54b3-124">id</span></span>|<span data-ttu-id="c54b3-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c54b3-125">String</span></span>|<span data-ttu-id="c54b3-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c54b3-126">Key of the entity.</span></span>|
|<span data-ttu-id="c54b3-127">displayName</span><span class="sxs-lookup"><span data-stu-id="c54b3-127">displayName</span></span>|<span data-ttu-id="c54b3-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c54b3-128">String</span></span>|<span data-ttu-id="c54b3-129">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c54b3-129">Name of the eBook.</span></span>|
|<span data-ttu-id="c54b3-130">description</span><span class="sxs-lookup"><span data-stu-id="c54b3-130">description</span></span>|<span data-ttu-id="c54b3-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c54b3-131">String</span></span>|<span data-ttu-id="c54b3-132">Descrição.</span><span class="sxs-lookup"><span data-stu-id="c54b3-132">Description.</span></span>|
|<span data-ttu-id="c54b3-133">publisher</span><span class="sxs-lookup"><span data-stu-id="c54b3-133">publisher</span></span>|<span data-ttu-id="c54b3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c54b3-134">String</span></span>|<span data-ttu-id="c54b3-135">Publicador.</span><span class="sxs-lookup"><span data-stu-id="c54b3-135">Publisher.</span></span>|
|<span data-ttu-id="c54b3-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c54b3-136">publishedDateTime</span></span>|<span data-ttu-id="c54b3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c54b3-137">DateTimeOffset</span></span>|<span data-ttu-id="c54b3-138">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="c54b3-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="c54b3-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="c54b3-139">largeCover</span></span>|[<span data-ttu-id="c54b3-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c54b3-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c54b3-141">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="c54b3-141">Book cover.</span></span>|
|<span data-ttu-id="c54b3-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c54b3-142">createdDateTime</span></span>|<span data-ttu-id="c54b3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c54b3-143">DateTimeOffset</span></span>|<span data-ttu-id="c54b3-144">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c54b3-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="c54b3-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c54b3-145">lastModifiedDateTime</span></span>|<span data-ttu-id="c54b3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c54b3-146">DateTimeOffset</span></span>|<span data-ttu-id="c54b3-147">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c54b3-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="c54b3-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c54b3-148">informationUrl</span></span>|<span data-ttu-id="c54b3-149">String</span><span class="sxs-lookup"><span data-stu-id="c54b3-149">String</span></span>|<span data-ttu-id="c54b3-150">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c54b3-150">The more information Url.</span></span>|
|<span data-ttu-id="c54b3-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c54b3-151">privacyInformationUrl</span></span>|<span data-ttu-id="c54b3-152">String</span><span class="sxs-lookup"><span data-stu-id="c54b3-152">String</span></span>|<span data-ttu-id="c54b3-153">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c54b3-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c54b3-154">Relações</span><span class="sxs-lookup"><span data-stu-id="c54b3-154">Relationships</span></span>
|<span data-ttu-id="c54b3-155">Relação</span><span class="sxs-lookup"><span data-stu-id="c54b3-155">Relationship</span></span>|<span data-ttu-id="c54b3-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="c54b3-156">Type</span></span>|<span data-ttu-id="c54b3-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54b3-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c54b3-158">assignments</span><span class="sxs-lookup"><span data-stu-id="c54b3-158">assignments</span></span>|<span data-ttu-id="c54b3-159">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c54b3-159">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="c54b3-160">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c54b3-160">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="c54b3-161">installSummary</span><span class="sxs-lookup"><span data-stu-id="c54b3-161">installSummary</span></span>|[<span data-ttu-id="c54b3-162">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c54b3-162">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="c54b3-163">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c54b3-163">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="c54b3-164">deviceStates</span><span class="sxs-lookup"><span data-stu-id="c54b3-164">deviceStates</span></span>|<span data-ttu-id="c54b3-165">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="c54b3-165">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="c54b3-166">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c54b3-166">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="c54b3-167">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="c54b3-167">userStateSummary</span></span>|<span data-ttu-id="c54b3-168">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="c54b3-168">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="c54b3-169">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c54b3-169">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c54b3-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c54b3-170">JSON Representation</span></span>
<span data-ttu-id="c54b3-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c54b3-171">Here is a JSON representation of the resource.</span></span>
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









