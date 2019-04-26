---
title: Tipo de recurso managedAppOperation
description: Representa uma operação aplicada a um registro de aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 545cacaa5f5d4c065e681dea1604d0fa89036132
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554104"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="18a7c-103">Tipo de recurso managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="18a7c-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="18a7c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18a7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18a7c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18a7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a7c-106">Representa uma operação aplicada a um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a7c-106">Represents an operation applied against an app registration.</span></span>

## <a name="methods"></a><span data-ttu-id="18a7c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="18a7c-107">Methods</span></span>
|<span data-ttu-id="18a7c-108">Método</span><span class="sxs-lookup"><span data-stu-id="18a7c-108">Method</span></span>|<span data-ttu-id="18a7c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18a7c-109">Return Type</span></span>|<span data-ttu-id="18a7c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a7c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18a7c-111">Listar managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="18a7c-111">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="18a7c-112">Conjunto [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="18a7c-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="18a7c-113">Listar propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="18a7c-113">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="18a7c-114">Obter managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="18a7c-114">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="18a7c-115">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="18a7c-115">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="18a7c-116">Ler propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="18a7c-116">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="18a7c-117">Criar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="18a7c-117">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="18a7c-118">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="18a7c-118">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="18a7c-119">Criar um novo objeto de[managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="18a7c-119">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="18a7c-120">Excluir managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="18a7c-120">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="18a7c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18a7c-121">None</span></span>|<span data-ttu-id="18a7c-122">Excluir [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="18a7c-122">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="18a7c-123">Atualizar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="18a7c-123">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="18a7c-124">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="18a7c-124">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="18a7c-125">Atualizar as propriedades de um objeto de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="18a7c-125">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="18a7c-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18a7c-126">Properties</span></span>
|<span data-ttu-id="18a7c-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18a7c-127">Property</span></span>|<span data-ttu-id="18a7c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="18a7c-128">Type</span></span>|<span data-ttu-id="18a7c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a7c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18a7c-130">displayName</span><span class="sxs-lookup"><span data-stu-id="18a7c-130">displayName</span></span>|<span data-ttu-id="18a7c-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a7c-131">String</span></span>|<span data-ttu-id="18a7c-132">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="18a7c-132">The operation name.</span></span>|
|<span data-ttu-id="18a7c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18a7c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="18a7c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a7c-134">DateTimeOffset</span></span>|<span data-ttu-id="18a7c-135">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="18a7c-135">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="18a7c-136">state</span><span class="sxs-lookup"><span data-stu-id="18a7c-136">state</span></span>|<span data-ttu-id="18a7c-137">String</span><span class="sxs-lookup"><span data-stu-id="18a7c-137">String</span></span>|<span data-ttu-id="18a7c-138">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="18a7c-138">The current state of the operation</span></span>|
|<span data-ttu-id="18a7c-139">id</span><span class="sxs-lookup"><span data-stu-id="18a7c-139">id</span></span>|<span data-ttu-id="18a7c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a7c-140">String</span></span>|<span data-ttu-id="18a7c-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18a7c-141">Key of the entity.</span></span>|
|<span data-ttu-id="18a7c-142">versão</span><span class="sxs-lookup"><span data-stu-id="18a7c-142">version</span></span>|<span data-ttu-id="18a7c-143">String</span><span class="sxs-lookup"><span data-stu-id="18a7c-143">String</span></span>|<span data-ttu-id="18a7c-144">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="18a7c-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18a7c-145">Relações</span><span class="sxs-lookup"><span data-stu-id="18a7c-145">Relationships</span></span>
<span data-ttu-id="18a7c-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18a7c-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18a7c-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18a7c-147">JSON Representation</span></span>
<span data-ttu-id="18a7c-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18a7c-148">Here is a JSON representation of the resource.</span></span>
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





