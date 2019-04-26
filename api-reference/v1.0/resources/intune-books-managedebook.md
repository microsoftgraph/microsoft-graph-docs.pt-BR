---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6151c23bf05b076ade441f908a2810c80f45ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534357"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="48e9f-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="48e9f-103">managedEBook resource type</span></span>

> <span data-ttu-id="48e9f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48e9f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48e9f-105">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="48e9f-105">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="48e9f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="48e9f-106">Methods</span></span>
|<span data-ttu-id="48e9f-107">Método</span><span class="sxs-lookup"><span data-stu-id="48e9f-107">Method</span></span>|<span data-ttu-id="48e9f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48e9f-108">Return Type</span></span>|<span data-ttu-id="48e9f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e9f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="48e9f-110">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="48e9f-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="48e9f-111">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="48e9f-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="48e9f-112">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="48e9f-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="48e9f-113">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="48e9f-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="48e9f-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="48e9f-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="48e9f-115">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="48e9f-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="48e9f-116">ação assign</span><span class="sxs-lookup"><span data-stu-id="48e9f-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="48e9f-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="48e9f-117">None</span></span>|<span data-ttu-id="48e9f-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48e9f-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="48e9f-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48e9f-119">Properties</span></span>
|<span data-ttu-id="48e9f-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48e9f-120">Property</span></span>|<span data-ttu-id="48e9f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="48e9f-121">Type</span></span>|<span data-ttu-id="48e9f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e9f-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e9f-123">id</span><span class="sxs-lookup"><span data-stu-id="48e9f-123">id</span></span>|<span data-ttu-id="48e9f-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48e9f-124">String</span></span>|<span data-ttu-id="48e9f-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48e9f-125">Key of the entity.</span></span>|
|<span data-ttu-id="48e9f-126">displayName</span><span class="sxs-lookup"><span data-stu-id="48e9f-126">displayName</span></span>|<span data-ttu-id="48e9f-127">String</span><span class="sxs-lookup"><span data-stu-id="48e9f-127">String</span></span>|<span data-ttu-id="48e9f-128">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="48e9f-128">Name of the eBook.</span></span>|
|<span data-ttu-id="48e9f-129">description</span><span class="sxs-lookup"><span data-stu-id="48e9f-129">description</span></span>|<span data-ttu-id="48e9f-130">String</span><span class="sxs-lookup"><span data-stu-id="48e9f-130">String</span></span>|<span data-ttu-id="48e9f-131">Descrição.</span><span class="sxs-lookup"><span data-stu-id="48e9f-131">Description.</span></span>|
|<span data-ttu-id="48e9f-132">publisher</span><span class="sxs-lookup"><span data-stu-id="48e9f-132">publisher</span></span>|<span data-ttu-id="48e9f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48e9f-133">String</span></span>|<span data-ttu-id="48e9f-134">Publicador.</span><span class="sxs-lookup"><span data-stu-id="48e9f-134">Publisher.</span></span>|
|<span data-ttu-id="48e9f-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="48e9f-135">publishedDateTime</span></span>|<span data-ttu-id="48e9f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48e9f-136">DateTimeOffset</span></span>|<span data-ttu-id="48e9f-137">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="48e9f-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="48e9f-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="48e9f-138">largeCover</span></span>|[<span data-ttu-id="48e9f-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="48e9f-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="48e9f-140">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="48e9f-140">Book cover.</span></span>|
|<span data-ttu-id="48e9f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48e9f-141">createdDateTime</span></span>|<span data-ttu-id="48e9f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48e9f-142">DateTimeOffset</span></span>|<span data-ttu-id="48e9f-143">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="48e9f-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="48e9f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48e9f-144">lastModifiedDateTime</span></span>|<span data-ttu-id="48e9f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48e9f-145">DateTimeOffset</span></span>|<span data-ttu-id="48e9f-146">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="48e9f-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="48e9f-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="48e9f-147">informationUrl</span></span>|<span data-ttu-id="48e9f-148">String</span><span class="sxs-lookup"><span data-stu-id="48e9f-148">String</span></span>|<span data-ttu-id="48e9f-149">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="48e9f-149">The more information Url.</span></span>|
|<span data-ttu-id="48e9f-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="48e9f-150">privacyInformationUrl</span></span>|<span data-ttu-id="48e9f-151">String</span><span class="sxs-lookup"><span data-stu-id="48e9f-151">String</span></span>|<span data-ttu-id="48e9f-152">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="48e9f-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48e9f-153">Relações</span><span class="sxs-lookup"><span data-stu-id="48e9f-153">Relationships</span></span>
|<span data-ttu-id="48e9f-154">Relação</span><span class="sxs-lookup"><span data-stu-id="48e9f-154">Relationship</span></span>|<span data-ttu-id="48e9f-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="48e9f-155">Type</span></span>|<span data-ttu-id="48e9f-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e9f-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e9f-157">assignments</span><span class="sxs-lookup"><span data-stu-id="48e9f-157">assignments</span></span>|<span data-ttu-id="48e9f-158">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="48e9f-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="48e9f-159">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="48e9f-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="48e9f-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="48e9f-160">installSummary</span></span>|[<span data-ttu-id="48e9f-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="48e9f-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="48e9f-162">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="48e9f-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="48e9f-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="48e9f-163">deviceStates</span></span>|<span data-ttu-id="48e9f-164">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="48e9f-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="48e9f-165">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="48e9f-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="48e9f-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="48e9f-166">userStateSummary</span></span>|<span data-ttu-id="48e9f-167">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="48e9f-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="48e9f-168">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="48e9f-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48e9f-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48e9f-169">JSON Representation</span></span>
<span data-ttu-id="48e9f-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48e9f-170">Here is a JSON representation of the resource.</span></span>
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



