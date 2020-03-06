---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 66d0efae21a68bd14286af45c4c021dbf7ba96fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531003"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="9f297-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="9f297-103">managedEBook resource type</span></span>

<span data-ttu-id="9f297-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f297-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f297-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f297-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f297-106">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="9f297-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="9f297-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9f297-107">Methods</span></span>
|<span data-ttu-id="9f297-108">Método</span><span class="sxs-lookup"><span data-stu-id="9f297-108">Method</span></span>|<span data-ttu-id="9f297-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9f297-109">Return Type</span></span>|<span data-ttu-id="9f297-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f297-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f297-111">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="9f297-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="9f297-112">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="9f297-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="9f297-113">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="9f297-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="9f297-114">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="9f297-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="9f297-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="9f297-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="9f297-116">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="9f297-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="9f297-117">ação assign</span><span class="sxs-lookup"><span data-stu-id="9f297-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="9f297-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9f297-118">None</span></span>|<span data-ttu-id="9f297-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9f297-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9f297-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f297-120">Properties</span></span>
|<span data-ttu-id="9f297-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f297-121">Property</span></span>|<span data-ttu-id="9f297-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f297-122">Type</span></span>|<span data-ttu-id="9f297-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f297-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f297-124">id</span><span class="sxs-lookup"><span data-stu-id="9f297-124">id</span></span>|<span data-ttu-id="9f297-125">String</span><span class="sxs-lookup"><span data-stu-id="9f297-125">String</span></span>|<span data-ttu-id="9f297-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9f297-126">Key of the entity.</span></span>|
|<span data-ttu-id="9f297-127">displayName</span><span class="sxs-lookup"><span data-stu-id="9f297-127">displayName</span></span>|<span data-ttu-id="9f297-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f297-128">String</span></span>|<span data-ttu-id="9f297-129">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="9f297-129">Name of the eBook.</span></span>|
|<span data-ttu-id="9f297-130">description</span><span class="sxs-lookup"><span data-stu-id="9f297-130">description</span></span>|<span data-ttu-id="9f297-131">String</span><span class="sxs-lookup"><span data-stu-id="9f297-131">String</span></span>|<span data-ttu-id="9f297-132">Descrição.</span><span class="sxs-lookup"><span data-stu-id="9f297-132">Description.</span></span>|
|<span data-ttu-id="9f297-133">publisher</span><span class="sxs-lookup"><span data-stu-id="9f297-133">publisher</span></span>|<span data-ttu-id="9f297-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f297-134">String</span></span>|<span data-ttu-id="9f297-135">Publicador.</span><span class="sxs-lookup"><span data-stu-id="9f297-135">Publisher.</span></span>|
|<span data-ttu-id="9f297-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f297-136">publishedDateTime</span></span>|<span data-ttu-id="9f297-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f297-137">DateTimeOffset</span></span>|<span data-ttu-id="9f297-138">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="9f297-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="9f297-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="9f297-139">largeCover</span></span>|[<span data-ttu-id="9f297-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9f297-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9f297-141">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="9f297-141">Book cover.</span></span>|
|<span data-ttu-id="9f297-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f297-142">createdDateTime</span></span>|<span data-ttu-id="9f297-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f297-143">DateTimeOffset</span></span>|<span data-ttu-id="9f297-144">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9f297-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="9f297-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f297-145">lastModifiedDateTime</span></span>|<span data-ttu-id="9f297-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f297-146">DateTimeOffset</span></span>|<span data-ttu-id="9f297-147">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="9f297-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="9f297-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9f297-148">informationUrl</span></span>|<span data-ttu-id="9f297-149">String</span><span class="sxs-lookup"><span data-stu-id="9f297-149">String</span></span>|<span data-ttu-id="9f297-150">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9f297-150">The more information Url.</span></span>|
|<span data-ttu-id="9f297-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9f297-151">privacyInformationUrl</span></span>|<span data-ttu-id="9f297-152">String</span><span class="sxs-lookup"><span data-stu-id="9f297-152">String</span></span>|<span data-ttu-id="9f297-153">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9f297-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f297-154">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="9f297-154">Relationships</span></span>
|<span data-ttu-id="9f297-155">Relação</span><span class="sxs-lookup"><span data-stu-id="9f297-155">Relationship</span></span>|<span data-ttu-id="9f297-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f297-156">Type</span></span>|<span data-ttu-id="9f297-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f297-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f297-158">assignments</span><span class="sxs-lookup"><span data-stu-id="9f297-158">assignments</span></span>|<span data-ttu-id="9f297-159">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9f297-159">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="9f297-160">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="9f297-160">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="9f297-161">installSummary</span><span class="sxs-lookup"><span data-stu-id="9f297-161">installSummary</span></span>|[<span data-ttu-id="9f297-162">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9f297-162">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="9f297-163">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="9f297-163">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="9f297-164">deviceStates</span><span class="sxs-lookup"><span data-stu-id="9f297-164">deviceStates</span></span>|<span data-ttu-id="9f297-165">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="9f297-165">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="9f297-166">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="9f297-166">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="9f297-167">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="9f297-167">userStateSummary</span></span>|<span data-ttu-id="9f297-168">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9f297-168">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="9f297-169">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="9f297-169">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f297-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f297-170">JSON Representation</span></span>
<span data-ttu-id="9f297-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f297-171">Here is a JSON representation of the resource.</span></span>
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




