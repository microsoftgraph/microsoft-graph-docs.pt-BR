---
title: Tipo de recurso managedAppOperation
description: Representa uma operação aplicada a um registro de aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a8c7ee3f49ad9b98d680662834911c2d20984d8d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951793"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="97d3f-103">Tipo de recurso managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="97d3f-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="97d3f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="97d3f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97d3f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97d3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97d3f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="97d3f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97d3f-107">Representa uma operação aplicada a um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97d3f-107">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="97d3f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="97d3f-108">Methods</span></span>
|<span data-ttu-id="97d3f-109">Método</span><span class="sxs-lookup"><span data-stu-id="97d3f-109">Method</span></span>|<span data-ttu-id="97d3f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="97d3f-110">Return Type</span></span>|<span data-ttu-id="97d3f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="97d3f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97d3f-112">Listar managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="97d3f-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="97d3f-113">Conjunto [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="97d3f-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="97d3f-114">Listar propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="97d3f-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="97d3f-115">Obter managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="97d3f-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="97d3f-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="97d3f-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="97d3f-117">Ler propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="97d3f-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="97d3f-118">Criar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="97d3f-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="97d3f-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="97d3f-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="97d3f-120">Criar um novo objeto de[managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="97d3f-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="97d3f-121">Excluir managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="97d3f-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="97d3f-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97d3f-122">None</span></span>|<span data-ttu-id="97d3f-123">Excluir [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="97d3f-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="97d3f-124">Atualizar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="97d3f-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="97d3f-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="97d3f-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="97d3f-126">Atualizar as propriedades de um objeto de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="97d3f-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="97d3f-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97d3f-127">Properties</span></span>
|<span data-ttu-id="97d3f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97d3f-128">Property</span></span>|<span data-ttu-id="97d3f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="97d3f-129">Type</span></span>|<span data-ttu-id="97d3f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="97d3f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d3f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="97d3f-131">displayName</span></span>|<span data-ttu-id="97d3f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97d3f-132">String</span></span>|<span data-ttu-id="97d3f-133">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="97d3f-133">The operation name.</span></span>|
|<span data-ttu-id="97d3f-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97d3f-134">lastModifiedDateTime</span></span>|<span data-ttu-id="97d3f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d3f-135">DateTimeOffset</span></span>|<span data-ttu-id="97d3f-136">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="97d3f-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="97d3f-137">estado</span><span class="sxs-lookup"><span data-stu-id="97d3f-137">state</span></span>|<span data-ttu-id="97d3f-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97d3f-138">String</span></span>|<span data-ttu-id="97d3f-139">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="97d3f-139">The current state of the operation</span></span>|
|<span data-ttu-id="97d3f-140">id</span><span class="sxs-lookup"><span data-stu-id="97d3f-140">id</span></span>|<span data-ttu-id="97d3f-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97d3f-141">String</span></span>|<span data-ttu-id="97d3f-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="97d3f-142">Key of the entity.</span></span>|
|<span data-ttu-id="97d3f-143">version</span><span class="sxs-lookup"><span data-stu-id="97d3f-143">version</span></span>|<span data-ttu-id="97d3f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97d3f-144">String</span></span>|<span data-ttu-id="97d3f-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="97d3f-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97d3f-146">Relações</span><span class="sxs-lookup"><span data-stu-id="97d3f-146">Relationships</span></span>
<span data-ttu-id="97d3f-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97d3f-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97d3f-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97d3f-148">JSON Representation</span></span>
<span data-ttu-id="97d3f-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97d3f-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```





