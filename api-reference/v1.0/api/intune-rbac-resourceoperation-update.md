---
title: Atualizar resourceOperation
description: Atualizar as propriedades de um objeto resourceOperation.
author: tfitzmac
ms.openlocfilehash: 98da602683c61313b11862bc5dc567f4a04e4268
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319730"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="cf5dc-103">Atualizar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="cf5dc-103">Update resourceOperation</span></span>

> <span data-ttu-id="cf5dc-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf5dc-105">Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="cf5dc-105">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf5dc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf5dc-106">Prerequisites</span></span>
<span data-ttu-id="cf5dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf5dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf5dc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf5dc-109">Permission type</span></span>|<span data-ttu-id="cf5dc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf5dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf5dc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf5dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf5dc-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf5dc-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cf5dc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf5dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf5dc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-114">Not supported.</span></span>|
|<span data-ttu-id="cf5dc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf5dc-115">Application</span></span>|<span data-ttu-id="cf5dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf5dc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf5dc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="cf5dc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5dc-118">Request headers</span></span>
|<span data-ttu-id="cf5dc-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf5dc-119">Header</span></span>|<span data-ttu-id="cf5dc-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cf5dc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf5dc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf5dc-121">Authorization</span></span>|<span data-ttu-id="cf5dc-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf5dc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cf5dc-123">Accept</span></span>|<span data-ttu-id="cf5dc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf5dc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf5dc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5dc-125">Request body</span></span>
<span data-ttu-id="cf5dc-126">No corpo da solicitação, forneça uma representação JSON do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="cf5dc-126">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="cf5dc-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="cf5dc-127">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="cf5dc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf5dc-128">Property</span></span>|<span data-ttu-id="cf5dc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf5dc-129">Type</span></span>|<span data-ttu-id="cf5dc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf5dc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf5dc-131">id</span><span class="sxs-lookup"><span data-stu-id="cf5dc-131">id</span></span>|<span data-ttu-id="cf5dc-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf5dc-132">String</span></span>|<span data-ttu-id="cf5dc-133">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-133">Key of the Resource Operation.</span></span> <span data-ttu-id="cf5dc-134">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="cf5dc-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="cf5dc-135">resourceName</span></span>|<span data-ttu-id="cf5dc-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf5dc-136">String</span></span>|<span data-ttu-id="cf5dc-137">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="cf5dc-138">actionName</span><span class="sxs-lookup"><span data-stu-id="cf5dc-138">actionName</span></span>|<span data-ttu-id="cf5dc-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf5dc-139">String</span></span>|<span data-ttu-id="cf5dc-140">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="cf5dc-141">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="cf5dc-142">description</span><span class="sxs-lookup"><span data-stu-id="cf5dc-142">description</span></span>|<span data-ttu-id="cf5dc-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf5dc-143">String</span></span>|<span data-ttu-id="cf5dc-144">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-144">Description of the resource operation.</span></span> <span data-ttu-id="cf5dc-145">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="cf5dc-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf5dc-146">Response</span></span>
<span data-ttu-id="cf5dc-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-147">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf5dc-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf5dc-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf5dc-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5dc-149">Request</span></span>
<span data-ttu-id="cf5dc-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf5dc-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf5dc-151">Response</span></span>
<span data-ttu-id="cf5dc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf5dc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



