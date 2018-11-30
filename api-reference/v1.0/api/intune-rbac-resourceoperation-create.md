---
title: Criar resourceOperation
description: Criar um novo objeto resourceOperation.
ms.openlocfilehash: 40f8c7175c5f6ad5e2885fe7e893bba118458be1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005348"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="05d49-103">Criar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="05d49-103">Create resourceOperation</span></span>

> <span data-ttu-id="05d49-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="05d49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05d49-105">Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="05d49-105">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05d49-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05d49-106">Prerequisites</span></span>
<span data-ttu-id="05d49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05d49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05d49-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05d49-109">Permission type</span></span>|<span data-ttu-id="05d49-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05d49-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05d49-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05d49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05d49-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05d49-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="05d49-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05d49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05d49-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05d49-114">Not supported.</span></span>|
|<span data-ttu-id="05d49-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05d49-115">Application</span></span>|<span data-ttu-id="05d49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05d49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05d49-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05d49-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="05d49-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05d49-118">Request headers</span></span>
|<span data-ttu-id="05d49-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05d49-119">Header</span></span>|<span data-ttu-id="05d49-120">Valor</span><span class="sxs-lookup"><span data-stu-id="05d49-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05d49-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="05d49-121">Authorization</span></span>|<span data-ttu-id="05d49-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05d49-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05d49-123">Accept</span><span class="sxs-lookup"><span data-stu-id="05d49-123">Accept</span></span>|<span data-ttu-id="05d49-124">application/json</span><span class="sxs-lookup"><span data-stu-id="05d49-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05d49-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05d49-125">Request body</span></span>
<span data-ttu-id="05d49-126">No corpo da solicitação, forneça uma representação JSON do objeto resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="05d49-126">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="05d49-127">A tabela a seguir mostra as propriedades que são necessárias ao criar resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="05d49-127">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="05d49-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05d49-128">Property</span></span>|<span data-ttu-id="05d49-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="05d49-129">Type</span></span>|<span data-ttu-id="05d49-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="05d49-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05d49-131">id</span><span class="sxs-lookup"><span data-stu-id="05d49-131">id</span></span>|<span data-ttu-id="05d49-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05d49-132">String</span></span>|<span data-ttu-id="05d49-133">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="05d49-133">Key of the Resource Operation.</span></span> <span data-ttu-id="05d49-134">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="05d49-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="05d49-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="05d49-135">resourceName</span></span>|<span data-ttu-id="05d49-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05d49-136">String</span></span>|<span data-ttu-id="05d49-137">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="05d49-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="05d49-138">actionName</span><span class="sxs-lookup"><span data-stu-id="05d49-138">actionName</span></span>|<span data-ttu-id="05d49-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05d49-139">String</span></span>|<span data-ttu-id="05d49-140">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="05d49-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="05d49-141">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="05d49-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="05d49-142">description</span><span class="sxs-lookup"><span data-stu-id="05d49-142">description</span></span>|<span data-ttu-id="05d49-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05d49-143">String</span></span>|<span data-ttu-id="05d49-144">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="05d49-144">Description of the resource operation.</span></span> <span data-ttu-id="05d49-145">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="05d49-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="05d49-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="05d49-146">Response</span></span>
<span data-ttu-id="05d49-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05d49-147">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05d49-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05d49-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="05d49-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05d49-149">Request</span></span>
<span data-ttu-id="05d49-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05d49-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="05d49-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="05d49-151">Response</span></span>
<span data-ttu-id="05d49-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05d49-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



