---
title: Criar resourceOperation
description: Criar um novo objeto resourceOperation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6790ce3486c25c85ec45750197f2394b7a8a544f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351410"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="eb24c-103">Criar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="eb24c-103">Create resourceOperation</span></span>

> <span data-ttu-id="eb24c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb24c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb24c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb24c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb24c-106">Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="eb24c-106">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb24c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb24c-107">Prerequisites</span></span>
<span data-ttu-id="eb24c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb24c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb24c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb24c-110">Permission type</span></span>|<span data-ttu-id="eb24c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb24c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb24c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb24c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb24c-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb24c-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="eb24c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb24c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb24c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb24c-115">Not supported.</span></span>|
|<span data-ttu-id="eb24c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb24c-116">Application</span></span>|<span data-ttu-id="eb24c-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb24c-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb24c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb24c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="eb24c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb24c-119">Request headers</span></span>
|<span data-ttu-id="eb24c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb24c-120">Header</span></span>|<span data-ttu-id="eb24c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb24c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb24c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb24c-122">Authorization</span></span>|<span data-ttu-id="eb24c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb24c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb24c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb24c-124">Accept</span></span>|<span data-ttu-id="eb24c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb24c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb24c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb24c-126">Request body</span></span>
<span data-ttu-id="eb24c-127">No corpo da solicitação, forneça uma representação JSON do objeto resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="eb24c-127">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="eb24c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="eb24c-128">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="eb24c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb24c-129">Property</span></span>|<span data-ttu-id="eb24c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb24c-130">Type</span></span>|<span data-ttu-id="eb24c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb24c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb24c-132">id</span><span class="sxs-lookup"><span data-stu-id="eb24c-132">id</span></span>|<span data-ttu-id="eb24c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb24c-133">String</span></span>|<span data-ttu-id="eb24c-134">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="eb24c-134">Key of the Resource Operation.</span></span> <span data-ttu-id="eb24c-135">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="eb24c-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="eb24c-136">recurso</span><span class="sxs-lookup"><span data-stu-id="eb24c-136">resource</span></span>|<span data-ttu-id="eb24c-137">String</span><span class="sxs-lookup"><span data-stu-id="eb24c-137">String</span></span>|<span data-ttu-id="eb24c-138">Categoria de recurso à qual essa operação pertence.</span><span class="sxs-lookup"><span data-stu-id="eb24c-138">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="eb24c-139">resourceName</span><span class="sxs-lookup"><span data-stu-id="eb24c-139">resourceName</span></span>|<span data-ttu-id="eb24c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb24c-140">String</span></span>|<span data-ttu-id="eb24c-141">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="eb24c-141">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="eb24c-142">actionName</span><span class="sxs-lookup"><span data-stu-id="eb24c-142">actionName</span></span>|<span data-ttu-id="eb24c-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb24c-143">String</span></span>|<span data-ttu-id="eb24c-144">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="eb24c-144">Type of action this operation is going to perform.</span></span> <span data-ttu-id="eb24c-145">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="eb24c-145">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="eb24c-146">descrição</span><span class="sxs-lookup"><span data-stu-id="eb24c-146">description</span></span>|<span data-ttu-id="eb24c-147">String</span><span class="sxs-lookup"><span data-stu-id="eb24c-147">String</span></span>|<span data-ttu-id="eb24c-148">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="eb24c-148">Description of the resource operation.</span></span> <span data-ttu-id="eb24c-149">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="eb24c-149">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="eb24c-150">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="eb24c-150">enabledForScopeValidation</span></span>|<span data-ttu-id="eb24c-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb24c-151">Boolean</span></span>|<span data-ttu-id="eb24c-152">Determina se a permissão é validada para os escopos definidos por atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="eb24c-152">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="eb24c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb24c-153">Response</span></span>
<span data-ttu-id="eb24c-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb24c-154">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb24c-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb24c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb24c-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb24c-156">Request</span></span>
<span data-ttu-id="eb24c-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb24c-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceOperations
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

### <a name="response"></a><span data-ttu-id="eb24c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb24c-158">Response</span></span>
<span data-ttu-id="eb24c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb24c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






