---
title: Atualizar resourceOperation
description: Atualizar as propriedades de um objeto resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 687f08a32347f18480523b5f06cf312131067370
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979659"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="13826-103">Atualizar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="13826-103">Update resourceOperation</span></span>

> <span data-ttu-id="13826-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13826-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13826-105">Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="13826-105">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13826-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13826-106">Prerequisites</span></span>
<span data-ttu-id="13826-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13826-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13826-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13826-109">Permission type</span></span>|<span data-ttu-id="13826-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13826-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13826-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13826-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13826-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13826-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="13826-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13826-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13826-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13826-114">Not supported.</span></span>|
|<span data-ttu-id="13826-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13826-115">Application</span></span>|<span data-ttu-id="13826-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13826-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13826-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13826-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="13826-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13826-118">Request headers</span></span>
|<span data-ttu-id="13826-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13826-119">Header</span></span>|<span data-ttu-id="13826-120">Valor</span><span class="sxs-lookup"><span data-stu-id="13826-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13826-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="13826-121">Authorization</span></span>|<span data-ttu-id="13826-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13826-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13826-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13826-123">Accept</span></span>|<span data-ttu-id="13826-124">application/json</span><span class="sxs-lookup"><span data-stu-id="13826-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13826-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13826-125">Request body</span></span>
<span data-ttu-id="13826-126">No corpo da solicitação, forneça uma representação JSON do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="13826-126">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="13826-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="13826-127">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="13826-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13826-128">Property</span></span>|<span data-ttu-id="13826-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="13826-129">Type</span></span>|<span data-ttu-id="13826-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="13826-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13826-131">id</span><span class="sxs-lookup"><span data-stu-id="13826-131">id</span></span>|<span data-ttu-id="13826-132">String</span><span class="sxs-lookup"><span data-stu-id="13826-132">String</span></span>|<span data-ttu-id="13826-133">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="13826-133">Key of the Resource Operation.</span></span> <span data-ttu-id="13826-134">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="13826-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="13826-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="13826-135">resourceName</span></span>|<span data-ttu-id="13826-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13826-136">String</span></span>|<span data-ttu-id="13826-137">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="13826-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="13826-138">actionName</span><span class="sxs-lookup"><span data-stu-id="13826-138">actionName</span></span>|<span data-ttu-id="13826-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13826-139">String</span></span>|<span data-ttu-id="13826-140">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="13826-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="13826-141">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="13826-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="13826-142">descrição</span><span class="sxs-lookup"><span data-stu-id="13826-142">description</span></span>|<span data-ttu-id="13826-143">String</span><span class="sxs-lookup"><span data-stu-id="13826-143">String</span></span>|<span data-ttu-id="13826-144">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="13826-144">Description of the resource operation.</span></span> <span data-ttu-id="13826-145">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="13826-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="13826-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="13826-146">Response</span></span>
<span data-ttu-id="13826-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13826-147">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13826-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13826-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="13826-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13826-149">Request</span></span>
<span data-ttu-id="13826-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13826-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13826-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="13826-151">Response</span></span>
<span data-ttu-id="13826-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13826-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



