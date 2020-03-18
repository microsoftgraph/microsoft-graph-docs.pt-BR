---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5a3894b183d8edae03091f65c535d504d9f9932
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761423"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="ec190-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="ec190-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="ec190-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec190-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec190-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec190-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec190-106">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ec190-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec190-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec190-107">Prerequisites</span></span>
<span data-ttu-id="ec190-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec190-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec190-110">Permission type</span></span>|<span data-ttu-id="ec190-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec190-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec190-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec190-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec190-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec190-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec190-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec190-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec190-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec190-115">Not supported.</span></span>|
|<span data-ttu-id="ec190-116">Application</span><span class="sxs-lookup"><span data-stu-id="ec190-116">Application</span></span>|<span data-ttu-id="ec190-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec190-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec190-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec190-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ec190-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec190-119">Request headers</span></span>
|<span data-ttu-id="ec190-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec190-120">Header</span></span>|<span data-ttu-id="ec190-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ec190-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec190-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec190-122">Authorization</span></span>|<span data-ttu-id="ec190-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec190-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec190-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec190-124">Accept</span></span>|<span data-ttu-id="ec190-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec190-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec190-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec190-126">Request body</span></span>
<span data-ttu-id="ec190-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="ec190-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="ec190-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="ec190-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="ec190-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec190-129">Property</span></span>|<span data-ttu-id="ec190-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec190-130">Type</span></span>|<span data-ttu-id="ec190-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec190-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec190-132">id</span><span class="sxs-lookup"><span data-stu-id="ec190-132">id</span></span>|<span data-ttu-id="ec190-133">String</span><span class="sxs-lookup"><span data-stu-id="ec190-133">String</span></span>|<span data-ttu-id="ec190-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ec190-134">Key of the entity.</span></span>|
|<span data-ttu-id="ec190-135">finalidade</span><span class="sxs-lookup"><span data-stu-id="ec190-135">intent</span></span>|[<span data-ttu-id="ec190-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="ec190-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ec190-137">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ec190-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="ec190-138">destino</span><span class="sxs-lookup"><span data-stu-id="ec190-138">target</span></span>|[<span data-ttu-id="ec190-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ec190-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ec190-140">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ec190-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="ec190-141">configurações</span><span class="sxs-lookup"><span data-stu-id="ec190-141">settings</span></span>|[<span data-ttu-id="ec190-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ec190-142">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="ec190-143">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ec190-143">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="ec190-144">source</span><span class="sxs-lookup"><span data-stu-id="ec190-144">source</span></span>|[<span data-ttu-id="ec190-145">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="ec190-145">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="ec190-146">O tipo de recurso que é a origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ec190-146">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="ec190-147">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="ec190-147">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="ec190-148">sourceId</span><span class="sxs-lookup"><span data-stu-id="ec190-148">sourceId</span></span>|<span data-ttu-id="ec190-149">String</span><span class="sxs-lookup"><span data-stu-id="ec190-149">String</span></span>|<span data-ttu-id="ec190-150">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ec190-150">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ec190-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec190-151">Response</span></span>
<span data-ttu-id="ec190-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec190-152">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec190-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec190-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec190-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec190-154">Request</span></span>
<span data-ttu-id="ec190-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec190-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="ec190-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec190-156">Response</span></span>
<span data-ttu-id="ec190-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec190-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




