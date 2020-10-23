---
title: Criar resourceOperation
description: Criar um novo objeto resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 324338018d68a9cdf9756290efeebe1a02e215e1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685545"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="971c6-103">Criar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="971c6-103">Create resourceOperation</span></span>

<span data-ttu-id="971c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="971c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="971c6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="971c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="971c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="971c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="971c6-107">Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="971c6-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="971c6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="971c6-108">Prerequisites</span></span>
<span data-ttu-id="971c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="971c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="971c6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="971c6-111">Permission type</span></span>|<span data-ttu-id="971c6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="971c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="971c6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="971c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="971c6-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="971c6-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="971c6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="971c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="971c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="971c6-116">Not supported.</span></span>|
|<span data-ttu-id="971c6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="971c6-117">Application</span></span>|<span data-ttu-id="971c6-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="971c6-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="971c6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="971c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="971c6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="971c6-120">Request headers</span></span>
|<span data-ttu-id="971c6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="971c6-121">Header</span></span>|<span data-ttu-id="971c6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="971c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="971c6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="971c6-123">Authorization</span></span>|<span data-ttu-id="971c6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="971c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="971c6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="971c6-125">Accept</span></span>|<span data-ttu-id="971c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="971c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="971c6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="971c6-127">Request body</span></span>
<span data-ttu-id="971c6-128">No corpo da solicitação, forneça uma representação JSON do objeto resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="971c6-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="971c6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="971c6-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="971c6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="971c6-130">Property</span></span>|<span data-ttu-id="971c6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="971c6-131">Type</span></span>|<span data-ttu-id="971c6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="971c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="971c6-133">id</span><span class="sxs-lookup"><span data-stu-id="971c6-133">id</span></span>|<span data-ttu-id="971c6-134">String</span><span class="sxs-lookup"><span data-stu-id="971c6-134">String</span></span>|<span data-ttu-id="971c6-135">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="971c6-135">Key of the Resource Operation.</span></span> <span data-ttu-id="971c6-136">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="971c6-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="971c6-137">recurso</span><span class="sxs-lookup"><span data-stu-id="971c6-137">resource</span></span>|<span data-ttu-id="971c6-138">String</span><span class="sxs-lookup"><span data-stu-id="971c6-138">String</span></span>|<span data-ttu-id="971c6-139">Categoria de recurso à qual essa operação pertence.</span><span class="sxs-lookup"><span data-stu-id="971c6-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="971c6-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="971c6-140">resourceName</span></span>|<span data-ttu-id="971c6-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="971c6-141">String</span></span>|<span data-ttu-id="971c6-142">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="971c6-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="971c6-143">actionName</span><span class="sxs-lookup"><span data-stu-id="971c6-143">actionName</span></span>|<span data-ttu-id="971c6-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="971c6-144">String</span></span>|<span data-ttu-id="971c6-145">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="971c6-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="971c6-146">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="971c6-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="971c6-147">description</span><span class="sxs-lookup"><span data-stu-id="971c6-147">description</span></span>|<span data-ttu-id="971c6-148">String</span><span class="sxs-lookup"><span data-stu-id="971c6-148">String</span></span>|<span data-ttu-id="971c6-149">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="971c6-149">Description of the resource operation.</span></span> <span data-ttu-id="971c6-150">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="971c6-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="971c6-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="971c6-151">enabledForScopeValidation</span></span>|<span data-ttu-id="971c6-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="971c6-152">Boolean</span></span>|<span data-ttu-id="971c6-153">Determina se a permissão é validada para os escopos definidos por atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="971c6-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="971c6-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="971c6-154">Response</span></span>
<span data-ttu-id="971c6-155">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="971c6-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="971c6-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="971c6-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="971c6-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="971c6-157">Request</span></span>
<span data-ttu-id="971c6-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="971c6-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="971c6-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="971c6-159">Response</span></span>
<span data-ttu-id="971c6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="971c6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





