---
title: Atualizar mobileAppAssignment
description: Atualizar as propriedades de um objeto mobileAppAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d8adb3390ed881ce3241ed746747d0d90a891e63
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177189"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="6f4d3-103">Atualizar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="6f4d3-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="6f4d3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f4d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f4d3-106">Atualizar as propriedades de um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6f4d3-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f4d3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f4d3-107">Prerequisites</span></span>
<span data-ttu-id="6f4d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f4d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f4d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f4d3-110">Permission type</span></span>|<span data-ttu-id="6f4d3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f4d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f4d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f4d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f4d3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f4d3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6f4d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f4d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f4d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-115">Not supported.</span></span>|
|<span data-ttu-id="6f4d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f4d3-116">Application</span></span>|<span data-ttu-id="6f4d3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f4d3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f4d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f4d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6f4d3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f4d3-119">Request headers</span></span>
|<span data-ttu-id="6f4d3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f4d3-120">Header</span></span>|<span data-ttu-id="6f4d3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6f4d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f4d3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f4d3-122">Authorization</span></span>|<span data-ttu-id="6f4d3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f4d3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f4d3-124">Accept</span></span>|<span data-ttu-id="6f4d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f4d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f4d3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f4d3-126">Request body</span></span>
<span data-ttu-id="6f4d3-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6f4d3-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="6f4d3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6f4d3-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="6f4d3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f4d3-129">Property</span></span>|<span data-ttu-id="6f4d3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f4d3-130">Type</span></span>|<span data-ttu-id="6f4d3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f4d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f4d3-132">id</span><span class="sxs-lookup"><span data-stu-id="6f4d3-132">id</span></span>|<span data-ttu-id="6f4d3-133">String</span><span class="sxs-lookup"><span data-stu-id="6f4d3-133">String</span></span>|<span data-ttu-id="6f4d3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-134">Key of the entity.</span></span>|
|<span data-ttu-id="6f4d3-135">finalidade</span><span class="sxs-lookup"><span data-stu-id="6f4d3-135">intent</span></span>|[<span data-ttu-id="6f4d3-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="6f4d3-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="6f4d3-137">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="6f4d3-138">destino</span><span class="sxs-lookup"><span data-stu-id="6f4d3-138">target</span></span>|[<span data-ttu-id="6f4d3-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6f4d3-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6f4d3-140">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="6f4d3-141">configurações</span><span class="sxs-lookup"><span data-stu-id="6f4d3-141">settings</span></span>|[<span data-ttu-id="6f4d3-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6f4d3-142">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="6f4d3-143">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="6f4d3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f4d3-144">Response</span></span>
<span data-ttu-id="6f4d3-145">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f4d3-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f4d3-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f4d3-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f4d3-147">Request</span></span>
<span data-ttu-id="6f4d3-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
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

### <a name="response"></a><span data-ttu-id="6f4d3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f4d3-149">Response</span></span>
<span data-ttu-id="6f4d3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f4d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




