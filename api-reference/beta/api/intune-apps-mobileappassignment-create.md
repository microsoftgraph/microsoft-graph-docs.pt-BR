---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e33e19764e8a4c49fa7b3e43b7f23cacfd8d9acd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39935923"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="aea02-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="aea02-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="aea02-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aea02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aea02-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aea02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aea02-106">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aea02-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aea02-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aea02-107">Prerequisites</span></span>
<span data-ttu-id="aea02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aea02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aea02-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aea02-110">Permission type</span></span>|<span data-ttu-id="aea02-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aea02-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aea02-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aea02-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aea02-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aea02-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aea02-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aea02-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aea02-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aea02-115">Not supported.</span></span>|
|<span data-ttu-id="aea02-116">Application</span><span class="sxs-lookup"><span data-stu-id="aea02-116">Application</span></span>|<span data-ttu-id="aea02-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aea02-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aea02-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aea02-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="aea02-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aea02-119">Request headers</span></span>
|<span data-ttu-id="aea02-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aea02-120">Header</span></span>|<span data-ttu-id="aea02-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aea02-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aea02-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aea02-122">Authorization</span></span>|<span data-ttu-id="aea02-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aea02-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aea02-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aea02-124">Accept</span></span>|<span data-ttu-id="aea02-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aea02-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aea02-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aea02-126">Request body</span></span>
<span data-ttu-id="aea02-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="aea02-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="aea02-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="aea02-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="aea02-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aea02-129">Property</span></span>|<span data-ttu-id="aea02-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="aea02-130">Type</span></span>|<span data-ttu-id="aea02-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aea02-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aea02-132">id</span><span class="sxs-lookup"><span data-stu-id="aea02-132">id</span></span>|<span data-ttu-id="aea02-133">String</span><span class="sxs-lookup"><span data-stu-id="aea02-133">String</span></span>|<span data-ttu-id="aea02-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aea02-134">Key of the entity.</span></span>|
|<span data-ttu-id="aea02-135">finalidade</span><span class="sxs-lookup"><span data-stu-id="aea02-135">intent</span></span>|[<span data-ttu-id="aea02-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="aea02-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="aea02-137">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="aea02-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="aea02-138">destino</span><span class="sxs-lookup"><span data-stu-id="aea02-138">target</span></span>|[<span data-ttu-id="aea02-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="aea02-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="aea02-140">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="aea02-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="aea02-141">configurações</span><span class="sxs-lookup"><span data-stu-id="aea02-141">settings</span></span>|[<span data-ttu-id="aea02-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="aea02-142">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="aea02-143">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="aea02-143">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="aea02-144">source</span><span class="sxs-lookup"><span data-stu-id="aea02-144">source</span></span>|[<span data-ttu-id="aea02-145">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="aea02-145">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="aea02-146">O tipo de recurso que é a origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="aea02-146">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="aea02-147">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="aea02-147">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="aea02-148">sourceId</span><span class="sxs-lookup"><span data-stu-id="aea02-148">sourceId</span></span>|<span data-ttu-id="aea02-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="aea02-149">String</span></span>|<span data-ttu-id="aea02-150">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="aea02-150">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="aea02-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="aea02-151">Response</span></span>
<span data-ttu-id="aea02-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aea02-152">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aea02-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aea02-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="aea02-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aea02-154">Request</span></span>
<span data-ttu-id="aea02-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aea02-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aea02-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="aea02-156">Response</span></span>
<span data-ttu-id="aea02-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aea02-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





