---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08bd5cc6f5630aca0ff5b35c5590875d259ad294
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422044"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="5f917-103">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="5f917-103">managedEBook resource type</span></span>

> <span data-ttu-id="5f917-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f917-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f917-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f917-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f917-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5f917-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f917-107">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="5f917-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="5f917-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5f917-108">Methods</span></span>
|<span data-ttu-id="5f917-109">Método</span><span class="sxs-lookup"><span data-stu-id="5f917-109">Method</span></span>|<span data-ttu-id="5f917-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5f917-110">Return Type</span></span>|<span data-ttu-id="5f917-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f917-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5f917-112">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="5f917-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="5f917-113">Coleção [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="5f917-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="5f917-114">Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5f917-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="5f917-115">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="5f917-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="5f917-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="5f917-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="5f917-117">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5f917-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="5f917-118">ação assign</span><span class="sxs-lookup"><span data-stu-id="5f917-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="5f917-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f917-119">None</span></span>|<span data-ttu-id="5f917-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5f917-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5f917-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f917-121">Properties</span></span>
|<span data-ttu-id="5f917-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f917-122">Property</span></span>|<span data-ttu-id="5f917-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f917-123">Type</span></span>|<span data-ttu-id="5f917-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f917-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f917-125">id</span><span class="sxs-lookup"><span data-stu-id="5f917-125">id</span></span>|<span data-ttu-id="5f917-126">String</span><span class="sxs-lookup"><span data-stu-id="5f917-126">String</span></span>|<span data-ttu-id="5f917-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5f917-127">Key of the entity.</span></span>|
|<span data-ttu-id="5f917-128">displayName</span><span class="sxs-lookup"><span data-stu-id="5f917-128">displayName</span></span>|<span data-ttu-id="5f917-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f917-129">String</span></span>|<span data-ttu-id="5f917-130">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5f917-130">Name of the eBook.</span></span>|
|<span data-ttu-id="5f917-131">description</span><span class="sxs-lookup"><span data-stu-id="5f917-131">description</span></span>|<span data-ttu-id="5f917-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f917-132">String</span></span>|<span data-ttu-id="5f917-133">Descrição.</span><span class="sxs-lookup"><span data-stu-id="5f917-133">Description.</span></span>|
|<span data-ttu-id="5f917-134">publisher</span><span class="sxs-lookup"><span data-stu-id="5f917-134">publisher</span></span>|<span data-ttu-id="5f917-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f917-135">String</span></span>|<span data-ttu-id="5f917-136">Publicador.</span><span class="sxs-lookup"><span data-stu-id="5f917-136">Publisher.</span></span>|
|<span data-ttu-id="5f917-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f917-137">publishedDateTime</span></span>|<span data-ttu-id="5f917-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f917-138">DateTimeOffset</span></span>|<span data-ttu-id="5f917-139">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="5f917-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="5f917-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="5f917-140">largeCover</span></span>|[<span data-ttu-id="5f917-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5f917-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5f917-142">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="5f917-142">Book cover.</span></span>|
|<span data-ttu-id="5f917-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f917-143">createdDateTime</span></span>|<span data-ttu-id="5f917-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f917-144">DateTimeOffset</span></span>|<span data-ttu-id="5f917-145">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5f917-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="5f917-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f917-146">lastModifiedDateTime</span></span>|<span data-ttu-id="5f917-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f917-147">DateTimeOffset</span></span>|<span data-ttu-id="5f917-148">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5f917-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="5f917-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5f917-149">informationUrl</span></span>|<span data-ttu-id="5f917-150">String</span><span class="sxs-lookup"><span data-stu-id="5f917-150">String</span></span>|<span data-ttu-id="5f917-151">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="5f917-151">The more information Url.</span></span>|
|<span data-ttu-id="5f917-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5f917-152">privacyInformationUrl</span></span>|<span data-ttu-id="5f917-153">String</span><span class="sxs-lookup"><span data-stu-id="5f917-153">String</span></span>|<span data-ttu-id="5f917-154">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="5f917-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f917-155">Relações</span><span class="sxs-lookup"><span data-stu-id="5f917-155">Relationships</span></span>
|<span data-ttu-id="5f917-156">Relação</span><span class="sxs-lookup"><span data-stu-id="5f917-156">Relationship</span></span>|<span data-ttu-id="5f917-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f917-157">Type</span></span>|<span data-ttu-id="5f917-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f917-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f917-159">categories</span><span class="sxs-lookup"><span data-stu-id="5f917-159">categories</span></span>|<span data-ttu-id="5f917-160">coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="5f917-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="5f917-161">A lista de categorias para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5f917-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="5f917-162">assignments</span><span class="sxs-lookup"><span data-stu-id="5f917-162">assignments</span></span>|<span data-ttu-id="5f917-163">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5f917-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="5f917-164">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5f917-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="5f917-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="5f917-165">installSummary</span></span>|[<span data-ttu-id="5f917-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5f917-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5f917-167">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="5f917-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="5f917-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="5f917-168">deviceStates</span></span>|<span data-ttu-id="5f917-169">Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="5f917-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="5f917-170">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5f917-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="5f917-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="5f917-171">userStateSummary</span></span>|<span data-ttu-id="5f917-172">Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="5f917-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="5f917-173">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5f917-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f917-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f917-174">JSON Representation</span></span>
<span data-ttu-id="5f917-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f917-175">Here is a JSON representation of the resource.</span></span>
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




