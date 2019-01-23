---
title: Atualizar mobileAppAssignment
description: Atualizar as propriedades de um objeto mobileAppAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bbedecc237e56022351fef82853fc3c2cb14bb91
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424319"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="d1a87-103">Atualizar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="d1a87-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="d1a87-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1a87-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1a87-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1a87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1a87-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d1a87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1a87-107">Atualizar as propriedades de um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d1a87-107">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1a87-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1a87-108">Prerequisites</span></span>
<span data-ttu-id="d1a87-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d1a87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d1a87-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1a87-111">Permission type</span></span>|<span data-ttu-id="d1a87-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1a87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1a87-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1a87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1a87-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1a87-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d1a87-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1a87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1a87-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1a87-116">Not supported.</span></span>|
|<span data-ttu-id="d1a87-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1a87-117">Application</span></span>|<span data-ttu-id="d1a87-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1a87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1a87-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1a87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d1a87-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1a87-120">Request headers</span></span>
|<span data-ttu-id="d1a87-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1a87-121">Header</span></span>|<span data-ttu-id="d1a87-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1a87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1a87-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1a87-123">Authorization</span></span>|<span data-ttu-id="d1a87-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1a87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1a87-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1a87-125">Accept</span></span>|<span data-ttu-id="d1a87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1a87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1a87-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1a87-127">Request body</span></span>
<span data-ttu-id="d1a87-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d1a87-128">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="d1a87-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d1a87-129">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="d1a87-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1a87-130">Property</span></span>|<span data-ttu-id="d1a87-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1a87-131">Type</span></span>|<span data-ttu-id="d1a87-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1a87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1a87-133">id</span><span class="sxs-lookup"><span data-stu-id="d1a87-133">id</span></span>|<span data-ttu-id="d1a87-134">String</span><span class="sxs-lookup"><span data-stu-id="d1a87-134">String</span></span>|<span data-ttu-id="d1a87-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d1a87-135">Key of the entity.</span></span>|
|<span data-ttu-id="d1a87-136">finalidade</span><span class="sxs-lookup"><span data-stu-id="d1a87-136">intent</span></span>|[<span data-ttu-id="d1a87-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="d1a87-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="d1a87-138">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="d1a87-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="d1a87-139">destino</span><span class="sxs-lookup"><span data-stu-id="d1a87-139">target</span></span>|[<span data-ttu-id="d1a87-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d1a87-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d1a87-141">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d1a87-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="d1a87-142">configurações</span><span class="sxs-lookup"><span data-stu-id="d1a87-142">settings</span></span>|[<span data-ttu-id="d1a87-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d1a87-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="d1a87-144">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d1a87-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="d1a87-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1a87-145">Response</span></span>
<span data-ttu-id="d1a87-146">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1a87-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1a87-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1a87-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1a87-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1a87-148">Request</span></span>
<span data-ttu-id="d1a87-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1a87-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1a87-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1a87-150">Response</span></span>
<span data-ttu-id="d1a87-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1a87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




