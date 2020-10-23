---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d303932765976cc8828fef5b256a7f7cf8e26482
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691481"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="61d84-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="61d84-103">managedEBook resource type</span></span>

<span data-ttu-id="61d84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61d84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61d84-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61d84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61d84-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61d84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61d84-107">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="61d84-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="61d84-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="61d84-108">Methods</span></span>
|<span data-ttu-id="61d84-109">Método</span><span class="sxs-lookup"><span data-stu-id="61d84-109">Method</span></span>|<span data-ttu-id="61d84-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="61d84-110">Return Type</span></span>|<span data-ttu-id="61d84-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d84-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61d84-112">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="61d84-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="61d84-113">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="61d84-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="61d84-114">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="61d84-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="61d84-115">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="61d84-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="61d84-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="61d84-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="61d84-117">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="61d84-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="61d84-118">ação assign</span><span class="sxs-lookup"><span data-stu-id="61d84-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="61d84-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="61d84-119">None</span></span>|<span data-ttu-id="61d84-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61d84-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="61d84-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61d84-121">Properties</span></span>
|<span data-ttu-id="61d84-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61d84-122">Property</span></span>|<span data-ttu-id="61d84-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="61d84-123">Type</span></span>|<span data-ttu-id="61d84-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d84-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d84-125">id</span><span class="sxs-lookup"><span data-stu-id="61d84-125">id</span></span>|<span data-ttu-id="61d84-126">String</span><span class="sxs-lookup"><span data-stu-id="61d84-126">String</span></span>|<span data-ttu-id="61d84-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="61d84-127">Key of the entity.</span></span>|
|<span data-ttu-id="61d84-128">displayName</span><span class="sxs-lookup"><span data-stu-id="61d84-128">displayName</span></span>|<span data-ttu-id="61d84-129">String</span><span class="sxs-lookup"><span data-stu-id="61d84-129">String</span></span>|<span data-ttu-id="61d84-130">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="61d84-130">Name of the eBook.</span></span>|
|<span data-ttu-id="61d84-131">description</span><span class="sxs-lookup"><span data-stu-id="61d84-131">description</span></span>|<span data-ttu-id="61d84-132">String</span><span class="sxs-lookup"><span data-stu-id="61d84-132">String</span></span>|<span data-ttu-id="61d84-133">Descrição.</span><span class="sxs-lookup"><span data-stu-id="61d84-133">Description.</span></span>|
|<span data-ttu-id="61d84-134">publisher</span><span class="sxs-lookup"><span data-stu-id="61d84-134">publisher</span></span>|<span data-ttu-id="61d84-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61d84-135">String</span></span>|<span data-ttu-id="61d84-136">Publicador.</span><span class="sxs-lookup"><span data-stu-id="61d84-136">Publisher.</span></span>|
|<span data-ttu-id="61d84-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="61d84-137">publishedDateTime</span></span>|<span data-ttu-id="61d84-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61d84-138">DateTimeOffset</span></span>|<span data-ttu-id="61d84-139">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="61d84-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="61d84-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="61d84-140">largeCover</span></span>|[<span data-ttu-id="61d84-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="61d84-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="61d84-142">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="61d84-142">Book cover.</span></span>|
|<span data-ttu-id="61d84-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61d84-143">createdDateTime</span></span>|<span data-ttu-id="61d84-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61d84-144">DateTimeOffset</span></span>|<span data-ttu-id="61d84-145">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="61d84-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="61d84-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61d84-146">lastModifiedDateTime</span></span>|<span data-ttu-id="61d84-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61d84-147">DateTimeOffset</span></span>|<span data-ttu-id="61d84-148">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="61d84-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="61d84-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="61d84-149">informationUrl</span></span>|<span data-ttu-id="61d84-150">String</span><span class="sxs-lookup"><span data-stu-id="61d84-150">String</span></span>|<span data-ttu-id="61d84-151">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="61d84-151">The more information Url.</span></span>|
|<span data-ttu-id="61d84-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="61d84-152">privacyInformationUrl</span></span>|<span data-ttu-id="61d84-153">String</span><span class="sxs-lookup"><span data-stu-id="61d84-153">String</span></span>|<span data-ttu-id="61d84-154">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="61d84-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61d84-155">Relações</span><span class="sxs-lookup"><span data-stu-id="61d84-155">Relationships</span></span>
|<span data-ttu-id="61d84-156">Relação</span><span class="sxs-lookup"><span data-stu-id="61d84-156">Relationship</span></span>|<span data-ttu-id="61d84-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="61d84-157">Type</span></span>|<span data-ttu-id="61d84-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d84-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d84-159">categories</span><span class="sxs-lookup"><span data-stu-id="61d84-159">categories</span></span>|<span data-ttu-id="61d84-160">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="61d84-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="61d84-161">A lista de categorias para este eBook.</span><span class="sxs-lookup"><span data-stu-id="61d84-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="61d84-162">assignments</span><span class="sxs-lookup"><span data-stu-id="61d84-162">assignments</span></span>|<span data-ttu-id="61d84-163">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="61d84-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="61d84-164">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="61d84-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="61d84-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="61d84-165">installSummary</span></span>|[<span data-ttu-id="61d84-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="61d84-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="61d84-167">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="61d84-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="61d84-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="61d84-168">deviceStates</span></span>|<span data-ttu-id="61d84-169">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="61d84-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="61d84-170">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="61d84-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="61d84-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="61d84-171">userStateSummary</span></span>|<span data-ttu-id="61d84-172">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="61d84-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="61d84-173">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="61d84-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61d84-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61d84-174">JSON Representation</span></span>
<span data-ttu-id="61d84-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61d84-175">Here is a JSON representation of the resource.</span></span>
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





