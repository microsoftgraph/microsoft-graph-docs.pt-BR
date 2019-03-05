---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7abf1163d5d323bf460b0a8dab3b54eb7ef8a2f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156697"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="a196f-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a196f-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="a196f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a196f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a196f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a196f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a196f-106">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a196f-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a196f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a196f-107">Prerequisites</span></span>
<span data-ttu-id="a196f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a196f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a196f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a196f-110">Permission type</span></span>|<span data-ttu-id="a196f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a196f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a196f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a196f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a196f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a196f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a196f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a196f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a196f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a196f-115">Not supported.</span></span>|
|<span data-ttu-id="a196f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a196f-116">Application</span></span>|<span data-ttu-id="a196f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a196f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a196f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a196f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a196f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a196f-119">Request headers</span></span>
|<span data-ttu-id="a196f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a196f-120">Header</span></span>|<span data-ttu-id="a196f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a196f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a196f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a196f-122">Authorization</span></span>|<span data-ttu-id="a196f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a196f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a196f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a196f-124">Accept</span></span>|<span data-ttu-id="a196f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a196f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a196f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a196f-126">Request body</span></span>
<span data-ttu-id="a196f-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="a196f-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="a196f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="a196f-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="a196f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a196f-129">Property</span></span>|<span data-ttu-id="a196f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a196f-130">Type</span></span>|<span data-ttu-id="a196f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a196f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a196f-132">id</span><span class="sxs-lookup"><span data-stu-id="a196f-132">id</span></span>|<span data-ttu-id="a196f-133">String</span><span class="sxs-lookup"><span data-stu-id="a196f-133">String</span></span>|<span data-ttu-id="a196f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a196f-134">Key of the entity.</span></span>|
|<span data-ttu-id="a196f-135">finalidade</span><span class="sxs-lookup"><span data-stu-id="a196f-135">intent</span></span>|[<span data-ttu-id="a196f-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="a196f-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="a196f-137">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="a196f-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="a196f-138">destino</span><span class="sxs-lookup"><span data-stu-id="a196f-138">target</span></span>|[<span data-ttu-id="a196f-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a196f-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a196f-140">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a196f-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="a196f-141">configurações</span><span class="sxs-lookup"><span data-stu-id="a196f-141">settings</span></span>|[<span data-ttu-id="a196f-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a196f-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="a196f-143">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a196f-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="a196f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a196f-144">Response</span></span>
<span data-ttu-id="a196f-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a196f-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a196f-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a196f-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="a196f-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a196f-147">Request</span></span>
<span data-ttu-id="a196f-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a196f-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="a196f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a196f-149">Response</span></span>
<span data-ttu-id="a196f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a196f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```




