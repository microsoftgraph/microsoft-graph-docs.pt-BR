---
title: Atualizar resourceOperation
description: Atualizar as propriedades de um objeto resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 857b93daef3b9a697e4ffa6ec5c206833d968024
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972032"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="ba6d5-103">Atualizar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ba6d5-103">Update resourceOperation</span></span>

<span data-ttu-id="ba6d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba6d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba6d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba6d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba6d5-107">Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ba6d5-107">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba6d5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba6d5-108">Prerequisites</span></span>
<span data-ttu-id="ba6d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba6d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba6d5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba6d5-111">Permission type</span></span>|<span data-ttu-id="ba6d5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba6d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba6d5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba6d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba6d5-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba6d5-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ba6d5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba6d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba6d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-116">Not supported.</span></span>|
|<span data-ttu-id="ba6d5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba6d5-117">Application</span></span>|<span data-ttu-id="ba6d5-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba6d5-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba6d5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba6d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="ba6d5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba6d5-120">Request headers</span></span>
|<span data-ttu-id="ba6d5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba6d5-121">Header</span></span>|<span data-ttu-id="ba6d5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ba6d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba6d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba6d5-123">Authorization</span></span>|<span data-ttu-id="ba6d5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba6d5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba6d5-125">Accept</span></span>|<span data-ttu-id="ba6d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba6d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba6d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba6d5-127">Request body</span></span>
<span data-ttu-id="ba6d5-128">No corpo da solicitação, forneça uma representação JSON do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ba6d5-128">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="ba6d5-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ba6d5-129">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="ba6d5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba6d5-130">Property</span></span>|<span data-ttu-id="ba6d5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba6d5-131">Type</span></span>|<span data-ttu-id="ba6d5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba6d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba6d5-133">id</span><span class="sxs-lookup"><span data-stu-id="ba6d5-133">id</span></span>|<span data-ttu-id="ba6d5-134">String</span><span class="sxs-lookup"><span data-stu-id="ba6d5-134">String</span></span>|<span data-ttu-id="ba6d5-135">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-135">Key of the Resource Operation.</span></span> <span data-ttu-id="ba6d5-136">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="ba6d5-137">recurso</span><span class="sxs-lookup"><span data-stu-id="ba6d5-137">resource</span></span>|<span data-ttu-id="ba6d5-138">String</span><span class="sxs-lookup"><span data-stu-id="ba6d5-138">String</span></span>|<span data-ttu-id="ba6d5-139">Categoria de recurso à qual essa operação pertence.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="ba6d5-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="ba6d5-140">resourceName</span></span>|<span data-ttu-id="ba6d5-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba6d5-141">String</span></span>|<span data-ttu-id="ba6d5-142">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="ba6d5-143">actionName</span><span class="sxs-lookup"><span data-stu-id="ba6d5-143">actionName</span></span>|<span data-ttu-id="ba6d5-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba6d5-144">String</span></span>|<span data-ttu-id="ba6d5-145">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="ba6d5-146">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="ba6d5-147">description</span><span class="sxs-lookup"><span data-stu-id="ba6d5-147">description</span></span>|<span data-ttu-id="ba6d5-148">String</span><span class="sxs-lookup"><span data-stu-id="ba6d5-148">String</span></span>|<span data-ttu-id="ba6d5-149">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-149">Description of the resource operation.</span></span> <span data-ttu-id="ba6d5-150">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="ba6d5-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="ba6d5-151">enabledForScopeValidation</span></span>|<span data-ttu-id="ba6d5-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba6d5-152">Boolean</span></span>|<span data-ttu-id="ba6d5-153">Determina se a permissão é validada para os escopos definidos por atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ba6d5-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba6d5-154">Response</span></span>
<span data-ttu-id="ba6d5-155">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-155">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba6d5-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba6d5-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba6d5-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba6d5-157">Request</span></span>
<span data-ttu-id="ba6d5-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 249

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```

### <a name="response"></a><span data-ttu-id="ba6d5-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba6d5-159">Response</span></span>
<span data-ttu-id="ba6d5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```






