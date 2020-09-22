---
title: Atualizar resourceOperation
description: Atualizar as propriedades de um objeto resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5e05a8b9bd78d6aaa7f11ea8bbf58efb313a22c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059401"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="db279-103">Atualizar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="db279-103">Update resourceOperation</span></span>

<span data-ttu-id="db279-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db279-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db279-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db279-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db279-106">Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="db279-106">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db279-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db279-107">Prerequisites</span></span>
<span data-ttu-id="db279-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db279-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db279-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db279-110">Permission type</span></span>|<span data-ttu-id="db279-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db279-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db279-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db279-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db279-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db279-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="db279-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db279-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db279-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db279-115">Not supported.</span></span>|
|<span data-ttu-id="db279-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db279-116">Application</span></span>|<span data-ttu-id="db279-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db279-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db279-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db279-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="db279-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db279-119">Request headers</span></span>
|<span data-ttu-id="db279-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db279-120">Header</span></span>|<span data-ttu-id="db279-121">Valor</span><span class="sxs-lookup"><span data-stu-id="db279-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db279-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="db279-122">Authorization</span></span>|<span data-ttu-id="db279-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db279-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db279-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db279-124">Accept</span></span>|<span data-ttu-id="db279-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db279-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db279-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db279-126">Request body</span></span>
<span data-ttu-id="db279-127">No corpo da solicitação, forneça uma representação JSON do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="db279-127">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="db279-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="db279-128">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="db279-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db279-129">Property</span></span>|<span data-ttu-id="db279-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="db279-130">Type</span></span>|<span data-ttu-id="db279-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="db279-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db279-132">id</span><span class="sxs-lookup"><span data-stu-id="db279-132">id</span></span>|<span data-ttu-id="db279-133">String</span><span class="sxs-lookup"><span data-stu-id="db279-133">String</span></span>|<span data-ttu-id="db279-134">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="db279-134">Key of the Resource Operation.</span></span> <span data-ttu-id="db279-135">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="db279-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="db279-136">resourceName</span><span class="sxs-lookup"><span data-stu-id="db279-136">resourceName</span></span>|<span data-ttu-id="db279-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db279-137">String</span></span>|<span data-ttu-id="db279-138">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="db279-138">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="db279-139">actionName</span><span class="sxs-lookup"><span data-stu-id="db279-139">actionName</span></span>|<span data-ttu-id="db279-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db279-140">String</span></span>|<span data-ttu-id="db279-141">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="db279-141">Type of action this operation is going to perform.</span></span> <span data-ttu-id="db279-142">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="db279-142">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="db279-143">description</span><span class="sxs-lookup"><span data-stu-id="db279-143">description</span></span>|<span data-ttu-id="db279-144">String</span><span class="sxs-lookup"><span data-stu-id="db279-144">String</span></span>|<span data-ttu-id="db279-145">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="db279-145">Description of the resource operation.</span></span> <span data-ttu-id="db279-146">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="db279-146">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="db279-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="db279-147">Response</span></span>
<span data-ttu-id="db279-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db279-148">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db279-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db279-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="db279-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db279-150">Request</span></span>
<span data-ttu-id="db279-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db279-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="db279-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="db279-152">Response</span></span>
<span data-ttu-id="db279-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db279-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```









