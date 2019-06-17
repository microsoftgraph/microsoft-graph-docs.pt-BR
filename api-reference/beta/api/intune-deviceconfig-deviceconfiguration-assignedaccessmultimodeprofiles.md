---
title: ação assignedAccessMultiModeProfiles
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49a8147631966bf93cb3e44cf08ed14854d5c14b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967997"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="0406b-103">ação assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="0406b-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="0406b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0406b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0406b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0406b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0406b-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0406b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0406b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0406b-107">Prerequisites</span></span>
<span data-ttu-id="0406b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0406b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0406b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0406b-110">Permission type</span></span>|<span data-ttu-id="0406b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0406b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0406b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0406b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0406b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0406b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0406b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0406b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0406b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0406b-115">Not supported.</span></span>|
|<span data-ttu-id="0406b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0406b-116">Application</span></span>|<span data-ttu-id="0406b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0406b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0406b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0406b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0406b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0406b-119">Request headers</span></span>
|<span data-ttu-id="0406b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0406b-120">Header</span></span>|<span data-ttu-id="0406b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0406b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0406b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0406b-122">Authorization</span></span>|<span data-ttu-id="0406b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0406b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0406b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0406b-124">Accept</span></span>|<span data-ttu-id="0406b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0406b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0406b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0406b-126">Request body</span></span>
<span data-ttu-id="0406b-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0406b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0406b-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0406b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0406b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0406b-129">Property</span></span>|<span data-ttu-id="0406b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0406b-130">Type</span></span>|<span data-ttu-id="0406b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0406b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0406b-132">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="0406b-132">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="0406b-133">coleção windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="0406b-133">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="0406b-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0406b-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0406b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0406b-135">Response</span></span>
<span data-ttu-id="0406b-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0406b-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0406b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0406b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="0406b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0406b-138">Request</span></span>
<span data-ttu-id="0406b-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0406b-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0406b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0406b-140">Response</span></span>
<span data-ttu-id="0406b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0406b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





