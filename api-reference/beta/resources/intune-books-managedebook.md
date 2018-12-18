---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: tfitzmac
ms.openlocfilehash: 7b826d7b0a11ce957a87154f276abc0e8168f45d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347142"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="70ce4-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="70ce4-103">managedEBook resource type</span></span>

> <span data-ttu-id="70ce4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="70ce4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70ce4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="70ce4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70ce4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="70ce4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70ce4-107">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="70ce4-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="70ce4-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="70ce4-108">Methods</span></span>
|<span data-ttu-id="70ce4-109">Método</span><span class="sxs-lookup"><span data-stu-id="70ce4-109">Method</span></span>|<span data-ttu-id="70ce4-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="70ce4-110">Return Type</span></span>|<span data-ttu-id="70ce4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="70ce4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="70ce4-112">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="70ce4-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="70ce4-113">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70ce4-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="70ce4-114">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="70ce4-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="70ce4-115">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="70ce4-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="70ce4-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="70ce4-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="70ce4-117">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="70ce4-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="70ce4-118">ação assign</span><span class="sxs-lookup"><span data-stu-id="70ce4-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="70ce4-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70ce4-119">None</span></span>|<span data-ttu-id="70ce4-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="70ce4-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="70ce4-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70ce4-121">Properties</span></span>
|<span data-ttu-id="70ce4-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70ce4-122">Property</span></span>|<span data-ttu-id="70ce4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="70ce4-123">Type</span></span>|<span data-ttu-id="70ce4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="70ce4-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70ce4-125">id</span><span class="sxs-lookup"><span data-stu-id="70ce4-125">id</span></span>|<span data-ttu-id="70ce4-126">String</span><span class="sxs-lookup"><span data-stu-id="70ce4-126">String</span></span>|<span data-ttu-id="70ce4-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="70ce4-127">Key of the entity.</span></span>|
|<span data-ttu-id="70ce4-128">displayName</span><span class="sxs-lookup"><span data-stu-id="70ce4-128">displayName</span></span>|<span data-ttu-id="70ce4-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70ce4-129">String</span></span>|<span data-ttu-id="70ce4-130">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="70ce4-130">Name of the eBook.</span></span>|
|<span data-ttu-id="70ce4-131">description</span><span class="sxs-lookup"><span data-stu-id="70ce4-131">description</span></span>|<span data-ttu-id="70ce4-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70ce4-132">String</span></span>|<span data-ttu-id="70ce4-133">Descrição.</span><span class="sxs-lookup"><span data-stu-id="70ce4-133">Description.</span></span>|
|<span data-ttu-id="70ce4-134">publisher</span><span class="sxs-lookup"><span data-stu-id="70ce4-134">publisher</span></span>|<span data-ttu-id="70ce4-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70ce4-135">String</span></span>|<span data-ttu-id="70ce4-136">Publicador.</span><span class="sxs-lookup"><span data-stu-id="70ce4-136">Publisher.</span></span>|
|<span data-ttu-id="70ce4-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="70ce4-137">publishedDateTime</span></span>|<span data-ttu-id="70ce4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70ce4-138">DateTimeOffset</span></span>|<span data-ttu-id="70ce4-139">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="70ce4-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="70ce4-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="70ce4-140">largeCover</span></span>|[<span data-ttu-id="70ce4-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="70ce4-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="70ce4-142">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="70ce4-142">Book cover.</span></span>|
|<span data-ttu-id="70ce4-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70ce4-143">createdDateTime</span></span>|<span data-ttu-id="70ce4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70ce4-144">DateTimeOffset</span></span>|<span data-ttu-id="70ce4-145">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="70ce4-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="70ce4-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70ce4-146">lastModifiedDateTime</span></span>|<span data-ttu-id="70ce4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70ce4-147">DateTimeOffset</span></span>|<span data-ttu-id="70ce4-148">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="70ce4-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="70ce4-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="70ce4-149">informationUrl</span></span>|<span data-ttu-id="70ce4-150">String</span><span class="sxs-lookup"><span data-stu-id="70ce4-150">String</span></span>|<span data-ttu-id="70ce4-151">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="70ce4-151">The more information Url.</span></span>|
|<span data-ttu-id="70ce4-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="70ce4-152">privacyInformationUrl</span></span>|<span data-ttu-id="70ce4-153">String</span><span class="sxs-lookup"><span data-stu-id="70ce4-153">String</span></span>|<span data-ttu-id="70ce4-154">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="70ce4-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70ce4-155">Relações</span><span class="sxs-lookup"><span data-stu-id="70ce4-155">Relationships</span></span>
|<span data-ttu-id="70ce4-156">Relação</span><span class="sxs-lookup"><span data-stu-id="70ce4-156">Relationship</span></span>|<span data-ttu-id="70ce4-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="70ce4-157">Type</span></span>|<span data-ttu-id="70ce4-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="70ce4-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70ce4-159">categories</span><span class="sxs-lookup"><span data-stu-id="70ce4-159">categories</span></span>|<span data-ttu-id="70ce4-160">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="70ce4-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="70ce4-161">A lista de categorias para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="70ce4-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="70ce4-162">assignments</span><span class="sxs-lookup"><span data-stu-id="70ce4-162">assignments</span></span>|<span data-ttu-id="70ce4-163">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="70ce4-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="70ce4-164">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="70ce4-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="70ce4-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="70ce4-165">installSummary</span></span>|[<span data-ttu-id="70ce4-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="70ce4-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="70ce4-167">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="70ce4-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="70ce4-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="70ce4-168">deviceStates</span></span>|<span data-ttu-id="70ce4-169">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="70ce4-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="70ce4-170">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="70ce4-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="70ce4-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="70ce4-171">userStateSummary</span></span>|<span data-ttu-id="70ce4-172">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="70ce4-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="70ce4-173">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="70ce4-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70ce4-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70ce4-174">JSON Representation</span></span>
<span data-ttu-id="70ce4-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70ce4-175">Here is a JSON representation of the resource.</span></span>
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





