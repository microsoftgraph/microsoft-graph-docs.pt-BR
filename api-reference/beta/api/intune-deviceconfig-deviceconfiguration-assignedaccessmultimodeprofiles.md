---
title: ação de assignedAccessMultiModeProfiles
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e52d3ee24223f56b0047b87f0d526329fd99ff79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944422"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="a7f3c-103">ação de assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="a7f3c-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="a7f3c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7f3c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7f3c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7f3c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a7f3c-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7f3c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7f3c-108">Prerequisites</span></span>
<span data-ttu-id="a7f3c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7f3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7f3c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7f3c-111">Permission type</span></span>|<span data-ttu-id="a7f3c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7f3c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7f3c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7f3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7f3c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7f3c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a7f3c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7f3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7f3c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-116">Not supported.</span></span>|
|<span data-ttu-id="a7f3c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7f3c-117">Application</span></span>|<span data-ttu-id="a7f3c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7f3c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7f3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a7f3c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7f3c-120">Request headers</span></span>
|<span data-ttu-id="a7f3c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7f3c-121">Header</span></span>|<span data-ttu-id="a7f3c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7f3c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7f3c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7f3c-123">Authorization</span></span>|<span data-ttu-id="a7f3c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7f3c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7f3c-125">Accept</span></span>|<span data-ttu-id="a7f3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7f3c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7f3c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7f3c-127">Request body</span></span>
<span data-ttu-id="a7f3c-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a7f3c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a7f3c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7f3c-130">Property</span></span>|<span data-ttu-id="a7f3c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7f3c-131">Type</span></span>|<span data-ttu-id="a7f3c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7f3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7f3c-133">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="a7f3c-133">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="a7f3c-134">coleção [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a7f3c-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) collection</span></span>|<span data-ttu-id="a7f3c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a7f3c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a7f3c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7f3c-136">Response</span></span>
<span data-ttu-id="a7f3c-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7f3c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7f3c-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7f3c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7f3c-139">Request</span></span>
<span data-ttu-id="a7f3c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7f3c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7f3c-141">Response</span></span>
<span data-ttu-id="a7f3c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7f3c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





