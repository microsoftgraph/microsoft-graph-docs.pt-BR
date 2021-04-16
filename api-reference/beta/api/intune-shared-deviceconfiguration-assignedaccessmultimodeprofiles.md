---
title: ação assignedAccessMultiModeProfiles
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 68a2f17e040c76ad51e244c8b385ae797f9aab23
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864274"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="e3c3f-103">ação assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="e3c3f-103">assignedAccessMultiModeProfiles action</span></span>

<span data-ttu-id="e3c3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3c3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3c3f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3c3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3c3f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3c3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3c3f-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3c3f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3c3f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3c3f-108">Prerequisites</span></span>
<span data-ttu-id="e3c3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3c3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3c3f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3c3f-111">Permission type</span></span>|<span data-ttu-id="e3c3f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3c3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3c3f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3c3f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e3c3f-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e3c3f-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e3c3f-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3c3f-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e3c3f-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3c3f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3c3f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3c3f-117">Not supported.</span></span>|
|<span data-ttu-id="e3c3f-118">Application</span><span class="sxs-lookup"><span data-stu-id="e3c3f-118">Application</span></span>||
| <span data-ttu-id="e3c3f-119">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e3c3f-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e3c3f-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3c3f-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3c3f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3c3f-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e3c3f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c3f-122">Request headers</span></span>
|<span data-ttu-id="e3c3f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3c3f-123">Header</span></span>|<span data-ttu-id="e3c3f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e3c3f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3c3f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3c3f-125">Authorization</span></span>|<span data-ttu-id="e3c3f-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3c3f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3c3f-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3c3f-127">Accept</span></span>|<span data-ttu-id="e3c3f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e3c3f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3c3f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c3f-129">Request body</span></span>
<span data-ttu-id="e3c3f-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e3c3f-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e3c3f-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e3c3f-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e3c3f-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3c3f-132">Property</span></span>|<span data-ttu-id="e3c3f-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3c3f-133">Type</span></span>|<span data-ttu-id="e3c3f-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c3f-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3c3f-135">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="e3c3f-135">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="e3c3f-136">Coleção windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="e3c3f-136">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="e3c3f-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3c3f-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e3c3f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c3f-138">Response</span></span>
<span data-ttu-id="e3c3f-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e3c3f-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e3c3f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3c3f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3c3f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c3f-141">Request</span></span>
<span data-ttu-id="e3c3f-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3c3f-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3c3f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c3f-143">Response</span></span>
<span data-ttu-id="e3c3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3c3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







