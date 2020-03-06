---
title: Atualizar mobileAppAssignment
description: Atualizar as propriedades de um objeto mobileAppAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 49c8b26de21e89cb6c7361f5c0ccd3348a48edd0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516027"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="9bb68-103">Atualizar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="9bb68-103">Update mobileAppAssignment</span></span>

<span data-ttu-id="9bb68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bb68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bb68-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bb68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bb68-106">Atualizar as propriedades de um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9bb68-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bb68-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bb68-107">Prerequisites</span></span>
<span data-ttu-id="9bb68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bb68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bb68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bb68-110">Permission type</span></span>|<span data-ttu-id="9bb68-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9bb68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bb68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bb68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bb68-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bb68-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9bb68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bb68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bb68-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bb68-115">Not supported.</span></span>|
|<span data-ttu-id="9bb68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bb68-116">Application</span></span>|<span data-ttu-id="9bb68-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bb68-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bb68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bb68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9bb68-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bb68-119">Request headers</span></span>
|<span data-ttu-id="9bb68-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bb68-120">Header</span></span>|<span data-ttu-id="9bb68-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9bb68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bb68-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bb68-122">Authorization</span></span>|<span data-ttu-id="9bb68-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bb68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bb68-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bb68-124">Accept</span></span>|<span data-ttu-id="9bb68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bb68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bb68-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bb68-126">Request body</span></span>
<span data-ttu-id="9bb68-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9bb68-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="9bb68-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9bb68-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="9bb68-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bb68-129">Property</span></span>|<span data-ttu-id="9bb68-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bb68-130">Type</span></span>|<span data-ttu-id="9bb68-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bb68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bb68-132">id</span><span class="sxs-lookup"><span data-stu-id="9bb68-132">id</span></span>|<span data-ttu-id="9bb68-133">String</span><span class="sxs-lookup"><span data-stu-id="9bb68-133">String</span></span>|<span data-ttu-id="9bb68-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9bb68-134">Key of the entity.</span></span>|
|<span data-ttu-id="9bb68-135">finalidade</span><span class="sxs-lookup"><span data-stu-id="9bb68-135">intent</span></span>|[<span data-ttu-id="9bb68-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="9bb68-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="9bb68-137">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="9bb68-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="9bb68-138">destino</span><span class="sxs-lookup"><span data-stu-id="9bb68-138">target</span></span>|[<span data-ttu-id="9bb68-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9bb68-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9bb68-140">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9bb68-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="9bb68-141">configurações</span><span class="sxs-lookup"><span data-stu-id="9bb68-141">settings</span></span>|[<span data-ttu-id="9bb68-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="9bb68-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="9bb68-143">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9bb68-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="9bb68-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bb68-144">Response</span></span>
<span data-ttu-id="9bb68-145">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bb68-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bb68-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bb68-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bb68-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bb68-147">Request</span></span>
<span data-ttu-id="9bb68-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bb68-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
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

### <a name="response"></a><span data-ttu-id="9bb68-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bb68-149">Response</span></span>
<span data-ttu-id="9bb68-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bb68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




