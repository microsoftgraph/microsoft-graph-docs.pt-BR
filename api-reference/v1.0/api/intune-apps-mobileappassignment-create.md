---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e2eea5bd9caa01430daa5e85a3fe7483d4e40aa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759739"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="0aa54-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="0aa54-103">Create mobileAppAssignment</span></span>

<span data-ttu-id="0aa54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aa54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0aa54-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0aa54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aa54-106">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0aa54-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0aa54-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0aa54-107">Prerequisites</span></span>
<span data-ttu-id="0aa54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aa54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aa54-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0aa54-110">Permission type</span></span>|<span data-ttu-id="0aa54-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0aa54-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aa54-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0aa54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0aa54-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aa54-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0aa54-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0aa54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aa54-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0aa54-115">Not supported.</span></span>|
|<span data-ttu-id="0aa54-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0aa54-116">Application</span></span>|<span data-ttu-id="0aa54-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aa54-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aa54-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0aa54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0aa54-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa54-119">Request headers</span></span>
|<span data-ttu-id="0aa54-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0aa54-120">Header</span></span>|<span data-ttu-id="0aa54-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0aa54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aa54-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0aa54-122">Authorization</span></span>|<span data-ttu-id="0aa54-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0aa54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aa54-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0aa54-124">Accept</span></span>|<span data-ttu-id="0aa54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0aa54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aa54-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa54-126">Request body</span></span>
<span data-ttu-id="0aa54-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="0aa54-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="0aa54-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="0aa54-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="0aa54-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0aa54-129">Property</span></span>|<span data-ttu-id="0aa54-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0aa54-130">Type</span></span>|<span data-ttu-id="0aa54-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0aa54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aa54-132">id</span><span class="sxs-lookup"><span data-stu-id="0aa54-132">id</span></span>|<span data-ttu-id="0aa54-133">String</span><span class="sxs-lookup"><span data-stu-id="0aa54-133">String</span></span>|<span data-ttu-id="0aa54-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0aa54-134">Key of the entity.</span></span>|
|<span data-ttu-id="0aa54-135">finalidade</span><span class="sxs-lookup"><span data-stu-id="0aa54-135">intent</span></span>|[<span data-ttu-id="0aa54-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="0aa54-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="0aa54-137">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="0aa54-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="0aa54-138">destino</span><span class="sxs-lookup"><span data-stu-id="0aa54-138">target</span></span>|[<span data-ttu-id="0aa54-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0aa54-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0aa54-140">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0aa54-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="0aa54-141">configurações</span><span class="sxs-lookup"><span data-stu-id="0aa54-141">settings</span></span>|[<span data-ttu-id="0aa54-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="0aa54-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="0aa54-143">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0aa54-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="0aa54-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aa54-144">Response</span></span>
<span data-ttu-id="0aa54-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0aa54-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aa54-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0aa54-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="0aa54-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa54-147">Request</span></span>
<span data-ttu-id="0aa54-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0aa54-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="0aa54-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aa54-149">Response</span></span>
<span data-ttu-id="0aa54-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0aa54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




