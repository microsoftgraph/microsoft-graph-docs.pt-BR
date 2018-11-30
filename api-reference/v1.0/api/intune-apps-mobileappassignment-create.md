---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
ms.openlocfilehash: f08335f131c97e67cb93d8dafcbce4c39bbef2e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003841"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="99c9b-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="99c9b-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="99c9b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="99c9b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99c9b-105">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="99c9b-105">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99c9b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99c9b-106">Prerequisites</span></span>
<span data-ttu-id="99c9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99c9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99c9b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99c9b-109">Permission type</span></span>|<span data-ttu-id="99c9b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99c9b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99c9b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99c9b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="99c9b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c9b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99c9b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99c9b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99c9b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99c9b-114">Not supported.</span></span>|
|<span data-ttu-id="99c9b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99c9b-115">Application</span></span>|<span data-ttu-id="99c9b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99c9b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99c9b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99c9b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="99c9b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99c9b-118">Request headers</span></span>
|<span data-ttu-id="99c9b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99c9b-119">Header</span></span>|<span data-ttu-id="99c9b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="99c9b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99c9b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="99c9b-121">Authorization</span></span>|<span data-ttu-id="99c9b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99c9b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99c9b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="99c9b-123">Accept</span></span>|<span data-ttu-id="99c9b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="99c9b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99c9b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99c9b-125">Request body</span></span>
<span data-ttu-id="99c9b-126">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="99c9b-126">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="99c9b-127">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="99c9b-127">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="99c9b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99c9b-128">Property</span></span>|<span data-ttu-id="99c9b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="99c9b-129">Type</span></span>|<span data-ttu-id="99c9b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="99c9b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c9b-131">id</span><span class="sxs-lookup"><span data-stu-id="99c9b-131">id</span></span>|<span data-ttu-id="99c9b-132">String</span><span class="sxs-lookup"><span data-stu-id="99c9b-132">String</span></span>|<span data-ttu-id="99c9b-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="99c9b-133">Key of the entity.</span></span>|
|<span data-ttu-id="99c9b-134">finalidade</span><span class="sxs-lookup"><span data-stu-id="99c9b-134">intent</span></span>|[<span data-ttu-id="99c9b-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="99c9b-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="99c9b-136">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="99c9b-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="99c9b-137">destino</span><span class="sxs-lookup"><span data-stu-id="99c9b-137">target</span></span>|[<span data-ttu-id="99c9b-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="99c9b-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="99c9b-139">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="99c9b-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="99c9b-140">configurações</span><span class="sxs-lookup"><span data-stu-id="99c9b-140">settings</span></span>|[<span data-ttu-id="99c9b-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="99c9b-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="99c9b-142">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="99c9b-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="99c9b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="99c9b-143">Response</span></span>
<span data-ttu-id="99c9b-144">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99c9b-144">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99c9b-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99c9b-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="99c9b-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99c9b-146">Request</span></span>
<span data-ttu-id="99c9b-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99c9b-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="99c9b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="99c9b-148">Response</span></span>
<span data-ttu-id="99c9b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99c9b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



