---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d743b425cb57a0b233ae83e5e044fd63fc85890e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755970"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="fceee-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="fceee-103">managedEBook resource type</span></span>

<span data-ttu-id="fceee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fceee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fceee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fceee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fceee-106">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="fceee-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="fceee-107">Methods</span><span class="sxs-lookup"><span data-stu-id="fceee-107">Methods</span></span>
|<span data-ttu-id="fceee-108">Método</span><span class="sxs-lookup"><span data-stu-id="fceee-108">Method</span></span>|<span data-ttu-id="fceee-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fceee-109">Return Type</span></span>|<span data-ttu-id="fceee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fceee-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fceee-111">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="fceee-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="fceee-112">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="fceee-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="fceee-113">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fceee-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="fceee-114">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="fceee-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="fceee-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="fceee-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="fceee-116">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fceee-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="fceee-117">ação assign</span><span class="sxs-lookup"><span data-stu-id="fceee-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="fceee-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="fceee-118">None</span></span>|<span data-ttu-id="fceee-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fceee-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fceee-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fceee-120">Properties</span></span>
|<span data-ttu-id="fceee-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fceee-121">Property</span></span>|<span data-ttu-id="fceee-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="fceee-122">Type</span></span>|<span data-ttu-id="fceee-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fceee-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fceee-124">id</span><span class="sxs-lookup"><span data-stu-id="fceee-124">id</span></span>|<span data-ttu-id="fceee-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fceee-125">String</span></span>|<span data-ttu-id="fceee-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fceee-126">Key of the entity.</span></span>|
|<span data-ttu-id="fceee-127">displayName</span><span class="sxs-lookup"><span data-stu-id="fceee-127">displayName</span></span>|<span data-ttu-id="fceee-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fceee-128">String</span></span>|<span data-ttu-id="fceee-129">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="fceee-129">Name of the eBook.</span></span>|
|<span data-ttu-id="fceee-130">descrição</span><span class="sxs-lookup"><span data-stu-id="fceee-130">description</span></span>|<span data-ttu-id="fceee-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fceee-131">String</span></span>|<span data-ttu-id="fceee-132">Descrição.</span><span class="sxs-lookup"><span data-stu-id="fceee-132">Description.</span></span>|
|<span data-ttu-id="fceee-133">publisher</span><span class="sxs-lookup"><span data-stu-id="fceee-133">publisher</span></span>|<span data-ttu-id="fceee-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fceee-134">String</span></span>|<span data-ttu-id="fceee-135">Publicador.</span><span class="sxs-lookup"><span data-stu-id="fceee-135">Publisher.</span></span>|
|<span data-ttu-id="fceee-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="fceee-136">publishedDateTime</span></span>|<span data-ttu-id="fceee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fceee-137">DateTimeOffset</span></span>|<span data-ttu-id="fceee-138">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="fceee-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="fceee-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="fceee-139">largeCover</span></span>|[<span data-ttu-id="fceee-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fceee-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fceee-141">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="fceee-141">Book cover.</span></span>|
|<span data-ttu-id="fceee-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fceee-142">createdDateTime</span></span>|<span data-ttu-id="fceee-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fceee-143">DateTimeOffset</span></span>|<span data-ttu-id="fceee-144">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fceee-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="fceee-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fceee-145">lastModifiedDateTime</span></span>|<span data-ttu-id="fceee-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fceee-146">DateTimeOffset</span></span>|<span data-ttu-id="fceee-147">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="fceee-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="fceee-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fceee-148">informationUrl</span></span>|<span data-ttu-id="fceee-149">String</span><span class="sxs-lookup"><span data-stu-id="fceee-149">String</span></span>|<span data-ttu-id="fceee-150">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="fceee-150">The more information Url.</span></span>|
|<span data-ttu-id="fceee-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fceee-151">privacyInformationUrl</span></span>|<span data-ttu-id="fceee-152">String</span><span class="sxs-lookup"><span data-stu-id="fceee-152">String</span></span>|<span data-ttu-id="fceee-153">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="fceee-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fceee-154">Relações</span><span class="sxs-lookup"><span data-stu-id="fceee-154">Relationships</span></span>
|<span data-ttu-id="fceee-155">Relação</span><span class="sxs-lookup"><span data-stu-id="fceee-155">Relationship</span></span>|<span data-ttu-id="fceee-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="fceee-156">Type</span></span>|<span data-ttu-id="fceee-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="fceee-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fceee-158">assignments</span><span class="sxs-lookup"><span data-stu-id="fceee-158">assignments</span></span>|<span data-ttu-id="fceee-159">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fceee-159">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="fceee-160">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="fceee-160">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="fceee-161">installSummary</span><span class="sxs-lookup"><span data-stu-id="fceee-161">installSummary</span></span>|[<span data-ttu-id="fceee-162">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="fceee-162">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="fceee-163">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="fceee-163">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="fceee-164">deviceStates</span><span class="sxs-lookup"><span data-stu-id="fceee-164">deviceStates</span></span>|<span data-ttu-id="fceee-165">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="fceee-165">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="fceee-166">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="fceee-166">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="fceee-167">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="fceee-167">userStateSummary</span></span>|<span data-ttu-id="fceee-168">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="fceee-168">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="fceee-169">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="fceee-169">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fceee-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fceee-170">JSON Representation</span></span>
<span data-ttu-id="fceee-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fceee-171">Here is a JSON representation of the resource.</span></span>
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




