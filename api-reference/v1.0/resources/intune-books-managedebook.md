---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 61a4098850f9b3b4a6b82f2fcee5d1ce89b0696d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830251"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="08ad7-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="08ad7-103">managedEBook resource type</span></span>

> <span data-ttu-id="08ad7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="08ad7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08ad7-105">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="08ad7-105">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="08ad7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="08ad7-106">Methods</span></span>
|<span data-ttu-id="08ad7-107">Método</span><span class="sxs-lookup"><span data-stu-id="08ad7-107">Method</span></span>|<span data-ttu-id="08ad7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="08ad7-108">Return Type</span></span>|<span data-ttu-id="08ad7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="08ad7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="08ad7-110">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="08ad7-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="08ad7-111">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="08ad7-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="08ad7-112">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="08ad7-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="08ad7-113">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="08ad7-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="08ad7-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="08ad7-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="08ad7-115">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="08ad7-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="08ad7-116">ação assign</span><span class="sxs-lookup"><span data-stu-id="08ad7-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="08ad7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08ad7-117">None</span></span>|<span data-ttu-id="08ad7-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="08ad7-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="08ad7-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08ad7-119">Properties</span></span>
|<span data-ttu-id="08ad7-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08ad7-120">Property</span></span>|<span data-ttu-id="08ad7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="08ad7-121">Type</span></span>|<span data-ttu-id="08ad7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="08ad7-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08ad7-123">id</span><span class="sxs-lookup"><span data-stu-id="08ad7-123">id</span></span>|<span data-ttu-id="08ad7-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08ad7-124">String</span></span>|<span data-ttu-id="08ad7-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="08ad7-125">Key of the entity.</span></span>|
|<span data-ttu-id="08ad7-126">displayName</span><span class="sxs-lookup"><span data-stu-id="08ad7-126">displayName</span></span>|<span data-ttu-id="08ad7-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08ad7-127">String</span></span>|<span data-ttu-id="08ad7-128">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="08ad7-128">Name of the eBook.</span></span>|
|<span data-ttu-id="08ad7-129">description</span><span class="sxs-lookup"><span data-stu-id="08ad7-129">description</span></span>|<span data-ttu-id="08ad7-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08ad7-130">String</span></span>|<span data-ttu-id="08ad7-131">Descrição.</span><span class="sxs-lookup"><span data-stu-id="08ad7-131">Description.</span></span>|
|<span data-ttu-id="08ad7-132">publisher</span><span class="sxs-lookup"><span data-stu-id="08ad7-132">publisher</span></span>|<span data-ttu-id="08ad7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08ad7-133">String</span></span>|<span data-ttu-id="08ad7-134">Publicador.</span><span class="sxs-lookup"><span data-stu-id="08ad7-134">Publisher.</span></span>|
|<span data-ttu-id="08ad7-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="08ad7-135">publishedDateTime</span></span>|<span data-ttu-id="08ad7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08ad7-136">DateTimeOffset</span></span>|<span data-ttu-id="08ad7-137">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="08ad7-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="08ad7-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="08ad7-138">largeCover</span></span>|[<span data-ttu-id="08ad7-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="08ad7-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="08ad7-140">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="08ad7-140">Book cover.</span></span>|
|<span data-ttu-id="08ad7-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08ad7-141">createdDateTime</span></span>|<span data-ttu-id="08ad7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08ad7-142">DateTimeOffset</span></span>|<span data-ttu-id="08ad7-143">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="08ad7-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="08ad7-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08ad7-144">lastModifiedDateTime</span></span>|<span data-ttu-id="08ad7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08ad7-145">DateTimeOffset</span></span>|<span data-ttu-id="08ad7-146">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="08ad7-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="08ad7-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="08ad7-147">informationUrl</span></span>|<span data-ttu-id="08ad7-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08ad7-148">String</span></span>|<span data-ttu-id="08ad7-149">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="08ad7-149">The more information Url.</span></span>|
|<span data-ttu-id="08ad7-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="08ad7-150">privacyInformationUrl</span></span>|<span data-ttu-id="08ad7-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08ad7-151">String</span></span>|<span data-ttu-id="08ad7-152">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="08ad7-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08ad7-153">Relações</span><span class="sxs-lookup"><span data-stu-id="08ad7-153">Relationships</span></span>
|<span data-ttu-id="08ad7-154">Relação</span><span class="sxs-lookup"><span data-stu-id="08ad7-154">Relationship</span></span>|<span data-ttu-id="08ad7-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="08ad7-155">Type</span></span>|<span data-ttu-id="08ad7-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="08ad7-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08ad7-157">assignments</span><span class="sxs-lookup"><span data-stu-id="08ad7-157">assignments</span></span>|<span data-ttu-id="08ad7-158">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="08ad7-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="08ad7-159">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="08ad7-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="08ad7-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="08ad7-160">installSummary</span></span>|[<span data-ttu-id="08ad7-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="08ad7-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="08ad7-162">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="08ad7-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="08ad7-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="08ad7-163">deviceStates</span></span>|<span data-ttu-id="08ad7-164">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="08ad7-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="08ad7-165">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="08ad7-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="08ad7-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="08ad7-166">userStateSummary</span></span>|<span data-ttu-id="08ad7-167">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08ad7-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="08ad7-168">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="08ad7-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08ad7-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08ad7-169">JSON Representation</span></span>
<span data-ttu-id="08ad7-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08ad7-170">Here is a JSON representation of the resource.</span></span>
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



