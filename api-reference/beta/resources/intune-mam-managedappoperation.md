---
title: Tipo de recurso managedAppOperation
description: Representa uma operação aplicada a um registro de aplicativo.
author: tfitzmac
ms.openlocfilehash: ab12d7e8d7014b1f7c1ea4d6e6dc8e8a81d804d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356907"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="b8735-103">Tipo de recurso managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b8735-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="b8735-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8735-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8735-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8735-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8735-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b8735-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8735-107">Representa uma operação aplicada a um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b8735-107">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="b8735-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b8735-108">Methods</span></span>
|<span data-ttu-id="b8735-109">Método</span><span class="sxs-lookup"><span data-stu-id="b8735-109">Method</span></span>|<span data-ttu-id="b8735-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b8735-110">Return Type</span></span>|<span data-ttu-id="b8735-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8735-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8735-112">Listar managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="b8735-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="b8735-113">Conjunto [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="b8735-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="b8735-114">Listar propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b8735-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="b8735-115">Obter managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b8735-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="b8735-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b8735-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="b8735-117">Ler propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b8735-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="b8735-118">Criar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b8735-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="b8735-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b8735-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="b8735-120">Criar um novo objeto de[managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b8735-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="b8735-121">Excluir managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b8735-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="b8735-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8735-122">None</span></span>|<span data-ttu-id="b8735-123">Excluir [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b8735-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="b8735-124">Atualizar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b8735-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="b8735-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b8735-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="b8735-126">Atualizar as propriedades de um objeto de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b8735-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8735-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8735-127">Properties</span></span>
|<span data-ttu-id="b8735-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8735-128">Property</span></span>|<span data-ttu-id="b8735-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8735-129">Type</span></span>|<span data-ttu-id="b8735-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8735-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8735-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b8735-131">displayName</span></span>|<span data-ttu-id="b8735-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8735-132">String</span></span>|<span data-ttu-id="b8735-133">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="b8735-133">The operation name.</span></span>|
|<span data-ttu-id="b8735-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8735-134">lastModifiedDateTime</span></span>|<span data-ttu-id="b8735-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8735-135">DateTimeOffset</span></span>|<span data-ttu-id="b8735-136">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="b8735-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="b8735-137">estado</span><span class="sxs-lookup"><span data-stu-id="b8735-137">state</span></span>|<span data-ttu-id="b8735-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8735-138">String</span></span>|<span data-ttu-id="b8735-139">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="b8735-139">The current state of the operation</span></span>|
|<span data-ttu-id="b8735-140">id</span><span class="sxs-lookup"><span data-stu-id="b8735-140">id</span></span>|<span data-ttu-id="b8735-141">String</span><span class="sxs-lookup"><span data-stu-id="b8735-141">String</span></span>|<span data-ttu-id="b8735-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b8735-142">Key of the entity.</span></span>|
|<span data-ttu-id="b8735-143">version</span><span class="sxs-lookup"><span data-stu-id="b8735-143">version</span></span>|<span data-ttu-id="b8735-144">String</span><span class="sxs-lookup"><span data-stu-id="b8735-144">String</span></span>|<span data-ttu-id="b8735-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b8735-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8735-146">Relações</span><span class="sxs-lookup"><span data-stu-id="b8735-146">Relationships</span></span>
<span data-ttu-id="b8735-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8735-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8735-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8735-148">JSON Representation</span></span>
<span data-ttu-id="b8735-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8735-149">Here is a JSON representation of the resource.</span></span>
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





