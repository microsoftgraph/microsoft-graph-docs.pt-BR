---
title: ação assignedAccessMultiModeProfiles
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9795d48fe744b78e301933d15aef48237e0e4343
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940079"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="f20ab-103">ação assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="f20ab-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="f20ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f20ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f20ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f20ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f20ab-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f20ab-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f20ab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f20ab-107">Prerequisites</span></span>
<span data-ttu-id="f20ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f20ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f20ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f20ab-110">Permission type</span></span>|<span data-ttu-id="f20ab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f20ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f20ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f20ab-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f20ab-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f20ab-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f20ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f20ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f20ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f20ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f20ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f20ab-116">Not supported.</span></span>|
|<span data-ttu-id="f20ab-117">Application</span><span class="sxs-lookup"><span data-stu-id="f20ab-117">Application</span></span>||
| <span data-ttu-id="f20ab-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f20ab-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f20ab-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f20ab-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f20ab-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f20ab-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f20ab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f20ab-121">Request headers</span></span>
|<span data-ttu-id="f20ab-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f20ab-122">Header</span></span>|<span data-ttu-id="f20ab-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f20ab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f20ab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f20ab-124">Authorization</span></span>|<span data-ttu-id="f20ab-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f20ab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f20ab-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f20ab-126">Accept</span></span>|<span data-ttu-id="f20ab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f20ab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f20ab-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f20ab-128">Request body</span></span>
<span data-ttu-id="f20ab-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f20ab-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f20ab-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f20ab-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f20ab-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f20ab-131">Property</span></span>|<span data-ttu-id="f20ab-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f20ab-132">Type</span></span>|<span data-ttu-id="f20ab-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f20ab-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f20ab-134">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="f20ab-134">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="f20ab-135">coleção windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="f20ab-135">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="f20ab-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f20ab-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f20ab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f20ab-137">Response</span></span>
<span data-ttu-id="f20ab-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f20ab-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f20ab-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f20ab-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="f20ab-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f20ab-140">Request</span></span>
<span data-ttu-id="f20ab-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f20ab-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f20ab-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f20ab-142">Response</span></span>
<span data-ttu-id="f20ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f20ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








