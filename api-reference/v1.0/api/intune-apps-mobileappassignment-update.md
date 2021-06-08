---
title: Atualizar mobileAppAssignment
description: Atualizar as propriedades de um objeto mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdc8e0145a782cc9a5eb87756542e8a7c5efcfb7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759725"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="f1478-103">Atualizar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="f1478-103">Update mobileAppAssignment</span></span>

<span data-ttu-id="f1478-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1478-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1478-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1478-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1478-106">Atualizar as propriedades de um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f1478-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1478-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1478-107">Prerequisites</span></span>
<span data-ttu-id="f1478-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1478-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1478-110">Permission type</span></span>|<span data-ttu-id="f1478-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1478-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1478-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1478-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1478-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1478-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f1478-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1478-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1478-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1478-115">Not supported.</span></span>|
|<span data-ttu-id="f1478-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1478-116">Application</span></span>|<span data-ttu-id="f1478-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1478-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1478-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1478-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f1478-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1478-119">Request headers</span></span>
|<span data-ttu-id="f1478-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1478-120">Header</span></span>|<span data-ttu-id="f1478-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f1478-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1478-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1478-122">Authorization</span></span>|<span data-ttu-id="f1478-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1478-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1478-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1478-124">Accept</span></span>|<span data-ttu-id="f1478-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1478-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1478-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1478-126">Request body</span></span>
<span data-ttu-id="f1478-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f1478-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="f1478-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f1478-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="f1478-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1478-129">Property</span></span>|<span data-ttu-id="f1478-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1478-130">Type</span></span>|<span data-ttu-id="f1478-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1478-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1478-132">id</span><span class="sxs-lookup"><span data-stu-id="f1478-132">id</span></span>|<span data-ttu-id="f1478-133">String</span><span class="sxs-lookup"><span data-stu-id="f1478-133">String</span></span>|<span data-ttu-id="f1478-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1478-134">Key of the entity.</span></span>|
|<span data-ttu-id="f1478-135">finalidade</span><span class="sxs-lookup"><span data-stu-id="f1478-135">intent</span></span>|[<span data-ttu-id="f1478-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="f1478-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="f1478-137">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="f1478-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="f1478-138">destino</span><span class="sxs-lookup"><span data-stu-id="f1478-138">target</span></span>|[<span data-ttu-id="f1478-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f1478-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f1478-140">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f1478-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="f1478-141">configurações</span><span class="sxs-lookup"><span data-stu-id="f1478-141">settings</span></span>|[<span data-ttu-id="f1478-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f1478-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="f1478-143">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f1478-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="f1478-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1478-144">Response</span></span>
<span data-ttu-id="f1478-145">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1478-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1478-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1478-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1478-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1478-147">Request</span></span>
<span data-ttu-id="f1478-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1478-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 324

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="f1478-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1478-149">Response</span></span>
<span data-ttu-id="f1478-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1478-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value"
  }
}
```




