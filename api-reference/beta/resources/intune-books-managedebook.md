---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3bf01c2115f4a0224ab09e59a9049324e82fa855
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834185"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="b25dd-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="b25dd-103">managedEBook resource type</span></span>

> <span data-ttu-id="b25dd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b25dd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b25dd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b25dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b25dd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b25dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b25dd-107">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b25dd-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="b25dd-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b25dd-108">Methods</span></span>
|<span data-ttu-id="b25dd-109">Método</span><span class="sxs-lookup"><span data-stu-id="b25dd-109">Method</span></span>|<span data-ttu-id="b25dd-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b25dd-110">Return Type</span></span>|<span data-ttu-id="b25dd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b25dd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b25dd-112">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="b25dd-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="b25dd-113">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="b25dd-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="b25dd-114">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b25dd-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="b25dd-115">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="b25dd-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="b25dd-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="b25dd-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="b25dd-117">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b25dd-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="b25dd-118">ação assign</span><span class="sxs-lookup"><span data-stu-id="b25dd-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="b25dd-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b25dd-119">None</span></span>|<span data-ttu-id="b25dd-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b25dd-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b25dd-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b25dd-121">Properties</span></span>
|<span data-ttu-id="b25dd-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b25dd-122">Property</span></span>|<span data-ttu-id="b25dd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b25dd-123">Type</span></span>|<span data-ttu-id="b25dd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b25dd-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b25dd-125">id</span><span class="sxs-lookup"><span data-stu-id="b25dd-125">id</span></span>|<span data-ttu-id="b25dd-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b25dd-126">String</span></span>|<span data-ttu-id="b25dd-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b25dd-127">Key of the entity.</span></span>|
|<span data-ttu-id="b25dd-128">displayName</span><span class="sxs-lookup"><span data-stu-id="b25dd-128">displayName</span></span>|<span data-ttu-id="b25dd-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b25dd-129">String</span></span>|<span data-ttu-id="b25dd-130">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="b25dd-130">Name of the eBook.</span></span>|
|<span data-ttu-id="b25dd-131">description</span><span class="sxs-lookup"><span data-stu-id="b25dd-131">description</span></span>|<span data-ttu-id="b25dd-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b25dd-132">String</span></span>|<span data-ttu-id="b25dd-133">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b25dd-133">Description.</span></span>|
|<span data-ttu-id="b25dd-134">publisher</span><span class="sxs-lookup"><span data-stu-id="b25dd-134">publisher</span></span>|<span data-ttu-id="b25dd-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b25dd-135">String</span></span>|<span data-ttu-id="b25dd-136">Publicador.</span><span class="sxs-lookup"><span data-stu-id="b25dd-136">Publisher.</span></span>|
|<span data-ttu-id="b25dd-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="b25dd-137">publishedDateTime</span></span>|<span data-ttu-id="b25dd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b25dd-138">DateTimeOffset</span></span>|<span data-ttu-id="b25dd-139">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="b25dd-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="b25dd-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="b25dd-140">largeCover</span></span>|[<span data-ttu-id="b25dd-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b25dd-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b25dd-142">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="b25dd-142">Book cover.</span></span>|
|<span data-ttu-id="b25dd-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b25dd-143">createdDateTime</span></span>|<span data-ttu-id="b25dd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b25dd-144">DateTimeOffset</span></span>|<span data-ttu-id="b25dd-145">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b25dd-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="b25dd-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b25dd-146">lastModifiedDateTime</span></span>|<span data-ttu-id="b25dd-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b25dd-147">DateTimeOffset</span></span>|<span data-ttu-id="b25dd-148">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="b25dd-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="b25dd-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b25dd-149">informationUrl</span></span>|<span data-ttu-id="b25dd-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b25dd-150">String</span></span>|<span data-ttu-id="b25dd-151">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b25dd-151">The more information Url.</span></span>|
|<span data-ttu-id="b25dd-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b25dd-152">privacyInformationUrl</span></span>|<span data-ttu-id="b25dd-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b25dd-153">String</span></span>|<span data-ttu-id="b25dd-154">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b25dd-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b25dd-155">Relações</span><span class="sxs-lookup"><span data-stu-id="b25dd-155">Relationships</span></span>
|<span data-ttu-id="b25dd-156">Relação</span><span class="sxs-lookup"><span data-stu-id="b25dd-156">Relationship</span></span>|<span data-ttu-id="b25dd-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="b25dd-157">Type</span></span>|<span data-ttu-id="b25dd-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="b25dd-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b25dd-159">categories</span><span class="sxs-lookup"><span data-stu-id="b25dd-159">categories</span></span>|<span data-ttu-id="b25dd-160">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b25dd-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="b25dd-161">A lista de categorias para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="b25dd-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="b25dd-162">assignments</span><span class="sxs-lookup"><span data-stu-id="b25dd-162">assignments</span></span>|<span data-ttu-id="b25dd-163">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b25dd-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="b25dd-164">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="b25dd-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="b25dd-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="b25dd-165">installSummary</span></span>|[<span data-ttu-id="b25dd-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b25dd-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="b25dd-167">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b25dd-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="b25dd-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="b25dd-168">deviceStates</span></span>|<span data-ttu-id="b25dd-169">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="b25dd-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="b25dd-170">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="b25dd-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="b25dd-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="b25dd-171">userStateSummary</span></span>|<span data-ttu-id="b25dd-172">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="b25dd-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="b25dd-173">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="b25dd-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b25dd-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b25dd-174">JSON Representation</span></span>
<span data-ttu-id="b25dd-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b25dd-175">Here is a JSON representation of the resource.</span></span>
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





