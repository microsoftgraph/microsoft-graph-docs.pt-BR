---
title: Criar resourceOperation
description: Criar um novo objeto resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ecbe52ac2c988967a121904e63d1bd6e00929a5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154149"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="b2fda-103">Criar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="b2fda-103">Create resourceOperation</span></span>

> <span data-ttu-id="b2fda-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2fda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2fda-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2fda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2fda-106">Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b2fda-106">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2fda-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2fda-107">Prerequisites</span></span>
<span data-ttu-id="b2fda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b2fda-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2fda-110">Permission type</span></span>|<span data-ttu-id="b2fda-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2fda-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2fda-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2fda-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2fda-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2fda-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b2fda-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2fda-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2fda-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2fda-115">Not supported.</span></span>|
|<span data-ttu-id="b2fda-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2fda-116">Application</span></span>|<span data-ttu-id="b2fda-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2fda-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2fda-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2fda-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="b2fda-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2fda-119">Request headers</span></span>
|<span data-ttu-id="b2fda-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2fda-120">Header</span></span>|<span data-ttu-id="b2fda-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2fda-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2fda-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2fda-122">Authorization</span></span>|<span data-ttu-id="b2fda-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2fda-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2fda-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2fda-124">Accept</span></span>|<span data-ttu-id="b2fda-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2fda-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2fda-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2fda-126">Request body</span></span>
<span data-ttu-id="b2fda-127">No corpo da solicitação, forneça uma representação JSON do objeto resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="b2fda-127">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="b2fda-128">A tabela a seguir mostra as propriedades que são necessárias ao criar resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="b2fda-128">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="b2fda-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2fda-129">Property</span></span>|<span data-ttu-id="b2fda-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2fda-130">Type</span></span>|<span data-ttu-id="b2fda-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2fda-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2fda-132">id</span><span class="sxs-lookup"><span data-stu-id="b2fda-132">id</span></span>|<span data-ttu-id="b2fda-133">String</span><span class="sxs-lookup"><span data-stu-id="b2fda-133">String</span></span>|<span data-ttu-id="b2fda-134">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="b2fda-134">Key of the Resource Operation.</span></span> <span data-ttu-id="b2fda-135">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b2fda-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="b2fda-136">recurso</span><span class="sxs-lookup"><span data-stu-id="b2fda-136">resource</span></span>|<span data-ttu-id="b2fda-137">String</span><span class="sxs-lookup"><span data-stu-id="b2fda-137">String</span></span>|<span data-ttu-id="b2fda-138">Categoria de recurso à qual essa operação pertence.</span><span class="sxs-lookup"><span data-stu-id="b2fda-138">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="b2fda-139">resourceName</span><span class="sxs-lookup"><span data-stu-id="b2fda-139">resourceName</span></span>|<span data-ttu-id="b2fda-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fda-140">String</span></span>|<span data-ttu-id="b2fda-141">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="b2fda-141">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="b2fda-142">actionName</span><span class="sxs-lookup"><span data-stu-id="b2fda-142">actionName</span></span>|<span data-ttu-id="b2fda-143">String</span><span class="sxs-lookup"><span data-stu-id="b2fda-143">String</span></span>|<span data-ttu-id="b2fda-144">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="b2fda-144">Type of action this operation is going to perform.</span></span> <span data-ttu-id="b2fda-145">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="b2fda-145">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="b2fda-146">description</span><span class="sxs-lookup"><span data-stu-id="b2fda-146">description</span></span>|<span data-ttu-id="b2fda-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fda-147">String</span></span>|<span data-ttu-id="b2fda-148">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="b2fda-148">Description of the resource operation.</span></span> <span data-ttu-id="b2fda-149">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b2fda-149">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="b2fda-150">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="b2fda-150">enabledForScopeValidation</span></span>|<span data-ttu-id="b2fda-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2fda-151">Boolean</span></span>|<span data-ttu-id="b2fda-152">Determina se a permissão é validada para os esCopos definidos por atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="b2fda-152">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="b2fda-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2fda-153">Response</span></span>
<span data-ttu-id="b2fda-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2fda-154">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2fda-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2fda-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2fda-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2fda-156">Request</span></span>
<span data-ttu-id="b2fda-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2fda-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2fda-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2fda-158">Response</span></span>
<span data-ttu-id="b2fda-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2fda-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




