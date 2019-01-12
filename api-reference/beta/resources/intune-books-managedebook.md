---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fd4fd3caef3aab90257805a48e53bee9c6b8764
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962594"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="6b8fe-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="6b8fe-103">managedEBook resource type</span></span>

> <span data-ttu-id="6b8fe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b8fe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b8fe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b8fe-107">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="6b8fe-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6b8fe-108">Methods</span></span>
|<span data-ttu-id="6b8fe-109">Método</span><span class="sxs-lookup"><span data-stu-id="6b8fe-109">Method</span></span>|<span data-ttu-id="6b8fe-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6b8fe-110">Return Type</span></span>|<span data-ttu-id="6b8fe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b8fe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b8fe-112">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="6b8fe-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="6b8fe-113">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="6b8fe-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="6b8fe-114">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="6b8fe-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="6b8fe-115">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="6b8fe-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="6b8fe-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="6b8fe-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="6b8fe-117">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="6b8fe-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="6b8fe-118">ação assign</span><span class="sxs-lookup"><span data-stu-id="6b8fe-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="6b8fe-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b8fe-119">None</span></span>|<span data-ttu-id="6b8fe-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6b8fe-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6b8fe-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b8fe-121">Properties</span></span>
|<span data-ttu-id="6b8fe-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b8fe-122">Property</span></span>|<span data-ttu-id="6b8fe-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b8fe-123">Type</span></span>|<span data-ttu-id="6b8fe-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b8fe-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b8fe-125">id</span><span class="sxs-lookup"><span data-stu-id="6b8fe-125">id</span></span>|<span data-ttu-id="6b8fe-126">String</span><span class="sxs-lookup"><span data-stu-id="6b8fe-126">String</span></span>|<span data-ttu-id="6b8fe-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-127">Key of the entity.</span></span>|
|<span data-ttu-id="6b8fe-128">displayName</span><span class="sxs-lookup"><span data-stu-id="6b8fe-128">displayName</span></span>|<span data-ttu-id="6b8fe-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b8fe-129">String</span></span>|<span data-ttu-id="6b8fe-130">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-130">Name of the eBook.</span></span>|
|<span data-ttu-id="6b8fe-131">description</span><span class="sxs-lookup"><span data-stu-id="6b8fe-131">description</span></span>|<span data-ttu-id="6b8fe-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b8fe-132">String</span></span>|<span data-ttu-id="6b8fe-133">Descrição.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-133">Description.</span></span>|
|<span data-ttu-id="6b8fe-134">publisher</span><span class="sxs-lookup"><span data-stu-id="6b8fe-134">publisher</span></span>|<span data-ttu-id="6b8fe-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b8fe-135">String</span></span>|<span data-ttu-id="6b8fe-136">Publicador.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-136">Publisher.</span></span>|
|<span data-ttu-id="6b8fe-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b8fe-137">publishedDateTime</span></span>|<span data-ttu-id="6b8fe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b8fe-138">DateTimeOffset</span></span>|<span data-ttu-id="6b8fe-139">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="6b8fe-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="6b8fe-140">largeCover</span></span>|[<span data-ttu-id="6b8fe-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6b8fe-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6b8fe-142">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-142">Book cover.</span></span>|
|<span data-ttu-id="6b8fe-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b8fe-143">createdDateTime</span></span>|<span data-ttu-id="6b8fe-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b8fe-144">DateTimeOffset</span></span>|<span data-ttu-id="6b8fe-145">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="6b8fe-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b8fe-146">lastModifiedDateTime</span></span>|<span data-ttu-id="6b8fe-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b8fe-147">DateTimeOffset</span></span>|<span data-ttu-id="6b8fe-148">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="6b8fe-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6b8fe-149">informationUrl</span></span>|<span data-ttu-id="6b8fe-150">String</span><span class="sxs-lookup"><span data-stu-id="6b8fe-150">String</span></span>|<span data-ttu-id="6b8fe-151">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-151">The more information Url.</span></span>|
|<span data-ttu-id="6b8fe-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6b8fe-152">privacyInformationUrl</span></span>|<span data-ttu-id="6b8fe-153">String</span><span class="sxs-lookup"><span data-stu-id="6b8fe-153">String</span></span>|<span data-ttu-id="6b8fe-154">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b8fe-155">Relações</span><span class="sxs-lookup"><span data-stu-id="6b8fe-155">Relationships</span></span>
|<span data-ttu-id="6b8fe-156">Relação</span><span class="sxs-lookup"><span data-stu-id="6b8fe-156">Relationship</span></span>|<span data-ttu-id="6b8fe-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b8fe-157">Type</span></span>|<span data-ttu-id="6b8fe-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b8fe-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b8fe-159">categories</span><span class="sxs-lookup"><span data-stu-id="6b8fe-159">categories</span></span>|<span data-ttu-id="6b8fe-160">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="6b8fe-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="6b8fe-161">A lista de categorias para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="6b8fe-162">assignments</span><span class="sxs-lookup"><span data-stu-id="6b8fe-162">assignments</span></span>|<span data-ttu-id="6b8fe-163">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6b8fe-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="6b8fe-164">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="6b8fe-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="6b8fe-165">installSummary</span></span>|[<span data-ttu-id="6b8fe-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6b8fe-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="6b8fe-167">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="6b8fe-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="6b8fe-168">deviceStates</span></span>|<span data-ttu-id="6b8fe-169">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="6b8fe-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="6b8fe-170">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="6b8fe-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="6b8fe-171">userStateSummary</span></span>|<span data-ttu-id="6b8fe-172">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="6b8fe-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="6b8fe-173">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b8fe-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b8fe-174">JSON Representation</span></span>
<span data-ttu-id="6b8fe-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b8fe-175">Here is a JSON representation of the resource.</span></span>
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





