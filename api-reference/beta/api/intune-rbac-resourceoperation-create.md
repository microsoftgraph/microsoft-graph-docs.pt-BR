---
title: Criar resourceOperation
description: Criar um novo objeto resourceOperation.
author: tfitzmac
ms.openlocfilehash: bc3b0c8193d77177b83f139827fad1a3a9686fb4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317833"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="0171f-103">Criar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="0171f-103">Create resourceOperation</span></span>

> <span data-ttu-id="0171f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0171f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0171f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0171f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0171f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0171f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0171f-107">Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0171f-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0171f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0171f-108">Prerequisites</span></span>
<span data-ttu-id="0171f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0171f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0171f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0171f-111">Permission type</span></span>|<span data-ttu-id="0171f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0171f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0171f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0171f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0171f-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0171f-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0171f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0171f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0171f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0171f-116">Not supported.</span></span>|
|<span data-ttu-id="0171f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0171f-117">Application</span></span>|<span data-ttu-id="0171f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0171f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0171f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0171f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="0171f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0171f-120">Request headers</span></span>
|<span data-ttu-id="0171f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0171f-121">Header</span></span>|<span data-ttu-id="0171f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0171f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0171f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0171f-123">Authorization</span></span>|<span data-ttu-id="0171f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0171f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0171f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0171f-125">Accept</span></span>|<span data-ttu-id="0171f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0171f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0171f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0171f-127">Request body</span></span>
<span data-ttu-id="0171f-128">No corpo da solicitação, forneça uma representação JSON do objeto resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="0171f-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="0171f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="0171f-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="0171f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0171f-130">Property</span></span>|<span data-ttu-id="0171f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0171f-131">Type</span></span>|<span data-ttu-id="0171f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0171f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0171f-133">id</span><span class="sxs-lookup"><span data-stu-id="0171f-133">id</span></span>|<span data-ttu-id="0171f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0171f-134">String</span></span>|<span data-ttu-id="0171f-135">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="0171f-135">Key of the Resource Operation.</span></span> <span data-ttu-id="0171f-136">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0171f-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="0171f-137">recurso</span><span class="sxs-lookup"><span data-stu-id="0171f-137">resource</span></span>|<span data-ttu-id="0171f-138">String</span><span class="sxs-lookup"><span data-stu-id="0171f-138">String</span></span>|<span data-ttu-id="0171f-139">Categoria de recurso ao qual esta operação pertence.</span><span class="sxs-lookup"><span data-stu-id="0171f-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="0171f-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="0171f-140">resourceName</span></span>|<span data-ttu-id="0171f-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0171f-141">String</span></span>|<span data-ttu-id="0171f-142">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="0171f-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="0171f-143">actionName</span><span class="sxs-lookup"><span data-stu-id="0171f-143">actionName</span></span>|<span data-ttu-id="0171f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0171f-144">String</span></span>|<span data-ttu-id="0171f-145">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="0171f-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="0171f-146">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="0171f-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="0171f-147">description</span><span class="sxs-lookup"><span data-stu-id="0171f-147">description</span></span>|<span data-ttu-id="0171f-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0171f-148">String</span></span>|<span data-ttu-id="0171f-149">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="0171f-149">Description of the resource operation.</span></span> <span data-ttu-id="0171f-150">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0171f-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="0171f-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="0171f-151">enabledForScopeValidation</span></span>|<span data-ttu-id="0171f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0171f-152">Boolean</span></span>|<span data-ttu-id="0171f-153">Determina se a permissão é validada para escopos definidos por atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="0171f-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="0171f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0171f-154">Response</span></span>
<span data-ttu-id="0171f-155">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0171f-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0171f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0171f-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="0171f-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0171f-157">Request</span></span>
<span data-ttu-id="0171f-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0171f-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0171f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="0171f-159">Response</span></span>
<span data-ttu-id="0171f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0171f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





