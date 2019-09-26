---
title: Atualizar resourceOperation
description: Atualizar as propriedades de um objeto resourceOperation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 435719ff8acc264fe36f431ea62dbb082519bfd4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189547"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="4d476-103">Atualizar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="4d476-103">Update resourceOperation</span></span>

> <span data-ttu-id="4d476-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d476-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d476-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d476-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d476-106">Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4d476-106">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d476-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d476-107">Prerequisites</span></span>
<span data-ttu-id="4d476-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d476-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d476-110">Permission type</span></span>|<span data-ttu-id="4d476-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4d476-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d476-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d476-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d476-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d476-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4d476-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d476-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d476-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d476-115">Not supported.</span></span>|
|<span data-ttu-id="4d476-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d476-116">Application</span></span>|<span data-ttu-id="4d476-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d476-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d476-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d476-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="4d476-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d476-119">Request headers</span></span>
|<span data-ttu-id="4d476-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d476-120">Header</span></span>|<span data-ttu-id="4d476-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4d476-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d476-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d476-122">Authorization</span></span>|<span data-ttu-id="4d476-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d476-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d476-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d476-124">Accept</span></span>|<span data-ttu-id="4d476-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d476-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d476-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d476-126">Request body</span></span>
<span data-ttu-id="4d476-127">No corpo da solicitação, forneça uma representação JSON do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4d476-127">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="4d476-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4d476-128">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="4d476-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d476-129">Property</span></span>|<span data-ttu-id="4d476-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d476-130">Type</span></span>|<span data-ttu-id="4d476-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d476-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d476-132">id</span><span class="sxs-lookup"><span data-stu-id="4d476-132">id</span></span>|<span data-ttu-id="4d476-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d476-133">String</span></span>|<span data-ttu-id="4d476-134">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="4d476-134">Key of the Resource Operation.</span></span> <span data-ttu-id="4d476-135">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="4d476-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="4d476-136">recurso</span><span class="sxs-lookup"><span data-stu-id="4d476-136">resource</span></span>|<span data-ttu-id="4d476-137">String</span><span class="sxs-lookup"><span data-stu-id="4d476-137">String</span></span>|<span data-ttu-id="4d476-138">Categoria de recurso à qual essa operação pertence.</span><span class="sxs-lookup"><span data-stu-id="4d476-138">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="4d476-139">resourceName</span><span class="sxs-lookup"><span data-stu-id="4d476-139">resourceName</span></span>|<span data-ttu-id="4d476-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d476-140">String</span></span>|<span data-ttu-id="4d476-141">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="4d476-141">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="4d476-142">actionName</span><span class="sxs-lookup"><span data-stu-id="4d476-142">actionName</span></span>|<span data-ttu-id="4d476-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d476-143">String</span></span>|<span data-ttu-id="4d476-144">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="4d476-144">Type of action this operation is going to perform.</span></span> <span data-ttu-id="4d476-145">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="4d476-145">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="4d476-146">descrição</span><span class="sxs-lookup"><span data-stu-id="4d476-146">description</span></span>|<span data-ttu-id="4d476-147">String</span><span class="sxs-lookup"><span data-stu-id="4d476-147">String</span></span>|<span data-ttu-id="4d476-148">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="4d476-148">Description of the resource operation.</span></span> <span data-ttu-id="4d476-149">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4d476-149">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="4d476-150">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="4d476-150">enabledForScopeValidation</span></span>|<span data-ttu-id="4d476-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d476-151">Boolean</span></span>|<span data-ttu-id="4d476-152">Determina se a permissão é validada para os escopos definidos por atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="4d476-152">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="4d476-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d476-153">Response</span></span>
<span data-ttu-id="4d476-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d476-154">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d476-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d476-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d476-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d476-156">Request</span></span>
<span data-ttu-id="4d476-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d476-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d476-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d476-158">Response</span></span>
<span data-ttu-id="4d476-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d476-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




