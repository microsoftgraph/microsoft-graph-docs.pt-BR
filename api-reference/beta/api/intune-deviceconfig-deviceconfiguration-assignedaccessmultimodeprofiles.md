---
title: ação assignedAccessMultiModeProfiles
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e439f28b74f3d5a8e2b71c0fc338ca5d5abfb6ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949409"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="dd8cf-103">ação assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="dd8cf-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="dd8cf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd8cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd8cf-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dd8cf-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd8cf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd8cf-107">Prerequisites</span></span>
<span data-ttu-id="dd8cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd8cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd8cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd8cf-110">Permission type</span></span>|<span data-ttu-id="dd8cf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd8cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd8cf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd8cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd8cf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd8cf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dd8cf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd8cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd8cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-115">Not supported.</span></span>|
|<span data-ttu-id="dd8cf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd8cf-116">Application</span></span>|<span data-ttu-id="dd8cf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd8cf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd8cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="dd8cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd8cf-119">Request headers</span></span>
|<span data-ttu-id="dd8cf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd8cf-120">Header</span></span>|<span data-ttu-id="dd8cf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dd8cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd8cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd8cf-122">Authorization</span></span>|<span data-ttu-id="dd8cf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd8cf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd8cf-124">Accept</span></span>|<span data-ttu-id="dd8cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd8cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd8cf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd8cf-126">Request body</span></span>
<span data-ttu-id="dd8cf-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dd8cf-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dd8cf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd8cf-129">Property</span></span>|<span data-ttu-id="dd8cf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd8cf-130">Type</span></span>|<span data-ttu-id="dd8cf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd8cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd8cf-132">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="dd8cf-132">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="dd8cf-133">coleção windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="dd8cf-133">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="dd8cf-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dd8cf-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dd8cf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd8cf-135">Response</span></span>
<span data-ttu-id="dd8cf-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dd8cf-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd8cf-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd8cf-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd8cf-138">Request</span></span>
<span data-ttu-id="dd8cf-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles

Content-type: application/json
Content-length: 528

{
  "assignedAccessMultiModeProfiles": [
    {
      "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
      "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
      "profileName": "Profile Name value",
      "showTaskBar": true,
      "appUserModelIds": [
        "App User Model Ids value"
      ],
      "desktopAppPaths": [
        "Desktop App Paths value"
      ],
      "userAccounts": [
        "User Accounts value"
      ],
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="dd8cf-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd8cf-140">Response</span></span>
<span data-ttu-id="dd8cf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd8cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





