---
title: Atualizar resourceOperation
description: Atualizar as propriedades de um objeto resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 332f8bdd76cde5d0f3bfe3065f7b30e692aba2ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461296"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="59490-103">Atualizar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="59490-103">Update resourceOperation</span></span>

<span data-ttu-id="59490-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59490-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59490-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59490-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59490-106">Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="59490-106">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59490-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59490-107">Prerequisites</span></span>
<span data-ttu-id="59490-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59490-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59490-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59490-110">Permission type</span></span>|<span data-ttu-id="59490-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59490-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59490-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59490-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59490-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59490-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="59490-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59490-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59490-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59490-115">Not supported.</span></span>|
|<span data-ttu-id="59490-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59490-116">Application</span></span>|<span data-ttu-id="59490-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59490-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59490-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59490-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="59490-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59490-119">Request headers</span></span>
|<span data-ttu-id="59490-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59490-120">Header</span></span>|<span data-ttu-id="59490-121">Valor</span><span class="sxs-lookup"><span data-stu-id="59490-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59490-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="59490-122">Authorization</span></span>|<span data-ttu-id="59490-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59490-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59490-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59490-124">Accept</span></span>|<span data-ttu-id="59490-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59490-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59490-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59490-126">Request body</span></span>
<span data-ttu-id="59490-127">No corpo da solicitação, forneça uma representação JSON do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="59490-127">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="59490-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="59490-128">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="59490-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59490-129">Property</span></span>|<span data-ttu-id="59490-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="59490-130">Type</span></span>|<span data-ttu-id="59490-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="59490-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59490-132">id</span><span class="sxs-lookup"><span data-stu-id="59490-132">id</span></span>|<span data-ttu-id="59490-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59490-133">String</span></span>|<span data-ttu-id="59490-134">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="59490-134">Key of the Resource Operation.</span></span> <span data-ttu-id="59490-135">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="59490-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="59490-136">resourceName</span><span class="sxs-lookup"><span data-stu-id="59490-136">resourceName</span></span>|<span data-ttu-id="59490-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59490-137">String</span></span>|<span data-ttu-id="59490-138">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="59490-138">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="59490-139">actionName</span><span class="sxs-lookup"><span data-stu-id="59490-139">actionName</span></span>|<span data-ttu-id="59490-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59490-140">String</span></span>|<span data-ttu-id="59490-141">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="59490-141">Type of action this operation is going to perform.</span></span> <span data-ttu-id="59490-142">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="59490-142">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="59490-143">description</span><span class="sxs-lookup"><span data-stu-id="59490-143">description</span></span>|<span data-ttu-id="59490-144">String</span><span class="sxs-lookup"><span data-stu-id="59490-144">String</span></span>|<span data-ttu-id="59490-145">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="59490-145">Description of the resource operation.</span></span> <span data-ttu-id="59490-146">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="59490-146">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="59490-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="59490-147">Response</span></span>
<span data-ttu-id="59490-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59490-148">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59490-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59490-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="59490-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59490-150">Request</span></span>
<span data-ttu-id="59490-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59490-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59490-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="59490-152">Response</span></span>
<span data-ttu-id="59490-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59490-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






