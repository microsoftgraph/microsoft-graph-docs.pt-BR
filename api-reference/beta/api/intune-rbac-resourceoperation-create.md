---
title: Criar resourceOperation
description: Criar um novo objeto resourceOperation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 92e1026e18c00978da8a1ac115e5d524adde75e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459783"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="1620c-103">Criar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1620c-103">Create resourceOperation</span></span>

<span data-ttu-id="1620c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1620c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1620c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1620c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1620c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1620c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1620c-107">Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="1620c-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1620c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1620c-108">Prerequisites</span></span>
<span data-ttu-id="1620c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1620c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1620c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1620c-111">Permission type</span></span>|<span data-ttu-id="1620c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1620c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1620c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1620c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1620c-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1620c-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="1620c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1620c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1620c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1620c-116">Not supported.</span></span>|
|<span data-ttu-id="1620c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1620c-117">Application</span></span>|<span data-ttu-id="1620c-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1620c-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1620c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1620c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="1620c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1620c-120">Request headers</span></span>
|<span data-ttu-id="1620c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1620c-121">Header</span></span>|<span data-ttu-id="1620c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1620c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1620c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1620c-123">Authorization</span></span>|<span data-ttu-id="1620c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1620c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1620c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1620c-125">Accept</span></span>|<span data-ttu-id="1620c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1620c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1620c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1620c-127">Request body</span></span>
<span data-ttu-id="1620c-128">No corpo da solicitação, forneça uma representação JSON do objeto resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="1620c-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="1620c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="1620c-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="1620c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1620c-130">Property</span></span>|<span data-ttu-id="1620c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1620c-131">Type</span></span>|<span data-ttu-id="1620c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1620c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1620c-133">id</span><span class="sxs-lookup"><span data-stu-id="1620c-133">id</span></span>|<span data-ttu-id="1620c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1620c-134">String</span></span>|<span data-ttu-id="1620c-135">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="1620c-135">Key of the Resource Operation.</span></span> <span data-ttu-id="1620c-136">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="1620c-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="1620c-137">recurso</span><span class="sxs-lookup"><span data-stu-id="1620c-137">resource</span></span>|<span data-ttu-id="1620c-138">String</span><span class="sxs-lookup"><span data-stu-id="1620c-138">String</span></span>|<span data-ttu-id="1620c-139">Categoria de recurso à qual essa operação pertence.</span><span class="sxs-lookup"><span data-stu-id="1620c-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="1620c-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="1620c-140">resourceName</span></span>|<span data-ttu-id="1620c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1620c-141">String</span></span>|<span data-ttu-id="1620c-142">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="1620c-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="1620c-143">actionName</span><span class="sxs-lookup"><span data-stu-id="1620c-143">actionName</span></span>|<span data-ttu-id="1620c-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1620c-144">String</span></span>|<span data-ttu-id="1620c-145">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="1620c-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="1620c-146">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="1620c-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="1620c-147">description</span><span class="sxs-lookup"><span data-stu-id="1620c-147">description</span></span>|<span data-ttu-id="1620c-148">String</span><span class="sxs-lookup"><span data-stu-id="1620c-148">String</span></span>|<span data-ttu-id="1620c-149">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="1620c-149">Description of the resource operation.</span></span> <span data-ttu-id="1620c-150">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1620c-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="1620c-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="1620c-151">enabledForScopeValidation</span></span>|<span data-ttu-id="1620c-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1620c-152">Boolean</span></span>|<span data-ttu-id="1620c-153">Determina se a permissão é validada para os escopos definidos por atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="1620c-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="1620c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="1620c-154">Response</span></span>
<span data-ttu-id="1620c-155">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1620c-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1620c-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1620c-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="1620c-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1620c-157">Request</span></span>
<span data-ttu-id="1620c-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1620c-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1620c-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="1620c-159">Response</span></span>
<span data-ttu-id="1620c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1620c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





