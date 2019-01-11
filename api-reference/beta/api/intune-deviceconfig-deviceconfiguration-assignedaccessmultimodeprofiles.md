---
title: ação de assignedAccessMultiModeProfiles
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 09183d5328b7dbbc92fa6052990e71b40df838ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828074"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="e2c16-103">ação de assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="e2c16-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="e2c16-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2c16-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2c16-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2c16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2c16-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e2c16-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2c16-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e2c16-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2c16-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2c16-108">Prerequisites</span></span>
<span data-ttu-id="e2c16-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2c16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2c16-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2c16-111">Permission type</span></span>|<span data-ttu-id="e2c16-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2c16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2c16-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2c16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2c16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2c16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e2c16-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2c16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2c16-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2c16-116">Not supported.</span></span>|
|<span data-ttu-id="e2c16-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2c16-117">Application</span></span>|<span data-ttu-id="e2c16-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2c16-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2c16-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2c16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e2c16-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2c16-120">Request headers</span></span>
|<span data-ttu-id="e2c16-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2c16-121">Header</span></span>|<span data-ttu-id="e2c16-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e2c16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2c16-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2c16-123">Authorization</span></span>|<span data-ttu-id="e2c16-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2c16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2c16-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2c16-125">Accept</span></span>|<span data-ttu-id="e2c16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2c16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2c16-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2c16-127">Request body</span></span>
<span data-ttu-id="e2c16-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e2c16-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e2c16-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e2c16-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e2c16-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2c16-130">Property</span></span>|<span data-ttu-id="e2c16-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2c16-131">Type</span></span>|<span data-ttu-id="e2c16-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2c16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2c16-133">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="e2c16-133">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="e2c16-134">coleção [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e2c16-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) collection</span></span>|<span data-ttu-id="e2c16-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e2c16-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e2c16-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2c16-136">Response</span></span>
<span data-ttu-id="e2c16-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e2c16-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e2c16-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2c16-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2c16-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2c16-139">Request</span></span>
<span data-ttu-id="e2c16-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2c16-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2c16-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2c16-141">Response</span></span>
<span data-ttu-id="e2c16-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2c16-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





