---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee72f668dacebe8c5567b57453fe5ef70b8f6540
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261135"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="c4fc7-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="c4fc7-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="c4fc7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4fc7-105">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c4fc7-105">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4fc7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4fc7-106">Prerequisites</span></span>
<span data-ttu-id="c4fc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4fc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c4fc7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4fc7-109">Permission type</span></span>|<span data-ttu-id="c4fc7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4fc7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4fc7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4fc7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4fc7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4fc7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c4fc7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4fc7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4fc7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-114">Not supported.</span></span>|
|<span data-ttu-id="c4fc7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4fc7-115">Application</span></span>|<span data-ttu-id="c4fc7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4fc7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4fc7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c4fc7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4fc7-118">Request headers</span></span>
|<span data-ttu-id="c4fc7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4fc7-119">Header</span></span>|<span data-ttu-id="c4fc7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c4fc7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4fc7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4fc7-121">Authorization</span></span>|<span data-ttu-id="c4fc7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4fc7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4fc7-123">Accept</span></span>|<span data-ttu-id="c4fc7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c4fc7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4fc7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4fc7-125">Request body</span></span>
<span data-ttu-id="c4fc7-126">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-126">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="c4fc7-127">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-127">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="c4fc7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4fc7-128">Property</span></span>|<span data-ttu-id="c4fc7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4fc7-129">Type</span></span>|<span data-ttu-id="c4fc7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4fc7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4fc7-131">id</span><span class="sxs-lookup"><span data-stu-id="c4fc7-131">id</span></span>|<span data-ttu-id="c4fc7-132">String</span><span class="sxs-lookup"><span data-stu-id="c4fc7-132">String</span></span>|<span data-ttu-id="c4fc7-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-133">Key of the entity.</span></span>|
|<span data-ttu-id="c4fc7-134">finalidade</span><span class="sxs-lookup"><span data-stu-id="c4fc7-134">intent</span></span>|[<span data-ttu-id="c4fc7-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="c4fc7-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="c4fc7-136">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="c4fc7-137">destino</span><span class="sxs-lookup"><span data-stu-id="c4fc7-137">target</span></span>|[<span data-ttu-id="c4fc7-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c4fc7-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c4fc7-139">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="c4fc7-140">configurações</span><span class="sxs-lookup"><span data-stu-id="c4fc7-140">settings</span></span>|[<span data-ttu-id="c4fc7-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="c4fc7-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="c4fc7-142">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="c4fc7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4fc7-143">Response</span></span>
<span data-ttu-id="c4fc7-144">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-144">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4fc7-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4fc7-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4fc7-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4fc7-146">Request</span></span>
<span data-ttu-id="c4fc7-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c4fc7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4fc7-148">Response</span></span>
<span data-ttu-id="c4fc7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4fc7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



