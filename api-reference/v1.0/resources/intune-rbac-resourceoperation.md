---
title: Tipo de recurso resourceOperation
description: Descreve o recurso resourceOperation (entidade) da API do Microsoft Graph (REST), que oferece suporte a fluxos de trabalho do Intune relacionados ao controle de acesso baseado em função (RBAC).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 95083bb1a3eb9f3c6e98deadd005aa6ef700555a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441605"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="0c545-103">Tipo de recurso resourceOperation</span><span class="sxs-lookup"><span data-stu-id="0c545-103">resourceOperation resource type</span></span>

<span data-ttu-id="0c545-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c545-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c545-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c545-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c545-106">Isso define uma operação ou ação que pode ser executada em um recurso (ou entidade) do Intune.</span><span class="sxs-lookup"><span data-stu-id="0c545-106">This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="0c545-107">As operações comuns são Ler, Excluir, Atualizar ou Criar.</span><span class="sxs-lookup"><span data-stu-id="0c545-107">Common operations are Read, Delete, Update or Create.</span></span>  <span data-ttu-id="0c545-108">Essas operações fornecem gerenciamento básico do recurso do Intune subjacente em si.</span><span class="sxs-lookup"><span data-stu-id="0c545-108">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="0c545-109">Em alguns casos, um recurso do Intune pode ter operações usadas pelo recurso para agir em combinação com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="0c545-109">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="0c545-110">Por exemplo, a operação Assign é usada para atribuir um recurso MobileApp a um grupo de segurança AAD.</span><span class="sxs-lookup"><span data-stu-id="0c545-110">For example, the Assign operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="0c545-111">Não é possível modificar as operações de recursos para funções internas. Isso define uma operação ou ação que pode ser executada em um recurso (ou entidade) do Intune.</span><span class="sxs-lookup"><span data-stu-id="0c545-111">Resource operations cannot be modified for built-in roles.This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="0c545-112">As operações comuns são Obter, Listar, Excluir, Atualizar ou Criar.</span><span class="sxs-lookup"><span data-stu-id="0c545-112">Common operations are Get, List, Delete, Update or Create.</span></span>  <span data-ttu-id="0c545-113">Essas operações fornecem gerenciamento básico do recurso do Intune subjacente em si.</span><span class="sxs-lookup"><span data-stu-id="0c545-113">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="0c545-114">Em alguns casos, um recurso do Intune pode ter operações usadas pelo recurso para agir em combinação com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="0c545-114">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="0c545-115">Por exemplo, a operação “Assign” é usada para atribuir um recurso MobileApp a um grupo de segurança AAD.</span><span class="sxs-lookup"><span data-stu-id="0c545-115">For example, the "Assign" operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="0c545-116">Não é possível modificar as operações de recursos para funções internas.</span><span class="sxs-lookup"><span data-stu-id="0c545-116">Resource operations cannot be modified for built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="0c545-117">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c545-117">Methods</span></span>
|<span data-ttu-id="0c545-118">Método</span><span class="sxs-lookup"><span data-stu-id="0c545-118">Method</span></span>|<span data-ttu-id="0c545-119">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0c545-119">Return Type</span></span>|<span data-ttu-id="0c545-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c545-120">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c545-121">Listar resourceOperations</span><span class="sxs-lookup"><span data-stu-id="0c545-121">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="0c545-122">Coleção [resourceOperation](../resources/intune-rbac-resourceoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0c545-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="0c545-123">Listar propriedades e relações dos objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0c545-123">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="0c545-124">Obter resourceOperation</span><span class="sxs-lookup"><span data-stu-id="0c545-124">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="0c545-125">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="0c545-125">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="0c545-126">Ler propriedades e relações do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0c545-126">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="0c545-127">Criar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="0c545-127">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="0c545-128">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="0c545-128">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="0c545-129">Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0c545-129">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="0c545-130">Excluir resourceOperation</span><span class="sxs-lookup"><span data-stu-id="0c545-130">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="0c545-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c545-131">None</span></span>|<span data-ttu-id="0c545-132">Excluir um [resourceOperation](../resources/intune-rbac-resourceoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0c545-132">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="0c545-133">Atualizar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="0c545-133">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="0c545-134">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="0c545-134">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="0c545-135">Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0c545-135">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c545-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c545-136">Properties</span></span>
|<span data-ttu-id="0c545-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c545-137">Property</span></span>|<span data-ttu-id="0c545-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c545-138">Type</span></span>|<span data-ttu-id="0c545-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c545-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c545-140">id</span><span class="sxs-lookup"><span data-stu-id="0c545-140">id</span></span>|<span data-ttu-id="0c545-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c545-141">String</span></span>|<span data-ttu-id="0c545-142">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="0c545-142">Key of the Resource Operation.</span></span> <span data-ttu-id="0c545-143">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0c545-143">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="0c545-144">resourceName</span><span class="sxs-lookup"><span data-stu-id="0c545-144">resourceName</span></span>|<span data-ttu-id="0c545-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c545-145">String</span></span>|<span data-ttu-id="0c545-146">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="0c545-146">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="0c545-147">actionName</span><span class="sxs-lookup"><span data-stu-id="0c545-147">actionName</span></span>|<span data-ttu-id="0c545-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c545-148">String</span></span>|<span data-ttu-id="0c545-149">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="0c545-149">Type of action this operation is going to perform.</span></span> <span data-ttu-id="0c545-150">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="0c545-150">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="0c545-151">description</span><span class="sxs-lookup"><span data-stu-id="0c545-151">description</span></span>|<span data-ttu-id="0c545-152">String</span><span class="sxs-lookup"><span data-stu-id="0c545-152">String</span></span>|<span data-ttu-id="0c545-153">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="0c545-153">Description of the resource operation.</span></span> <span data-ttu-id="0c545-154">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0c545-154">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c545-155">Relações</span><span class="sxs-lookup"><span data-stu-id="0c545-155">Relationships</span></span>
<span data-ttu-id="0c545-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c545-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c545-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c545-157">JSON Representation</span></span>
<span data-ttu-id="0c545-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c545-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```







