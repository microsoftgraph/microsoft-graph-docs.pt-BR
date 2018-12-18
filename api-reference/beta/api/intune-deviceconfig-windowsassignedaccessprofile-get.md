---
title: Obter windowsAssignedAccessProfile
description: Leia as propriedades e os relacionamentos do objeto windowsAssignedAccessProfile.
author: tfitzmac
ms.openlocfilehash: a4a4fd692c8147283950bb3a2d5de6ebebcd4173
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349760"
---
# <a name="get-windowsassignedaccessprofile"></a><span data-ttu-id="e7d59-103">Obter windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="e7d59-103">Get windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="e7d59-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7d59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7d59-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7d59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7d59-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e7d59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7d59-107">Leia as propriedades e os relacionamentos do objeto [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e7d59-107">Read properties and relationships of the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7d59-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7d59-108">Prerequisites</span></span>
<span data-ttu-id="e7d59-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d59-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7d59-111">Permission type</span></span>|<span data-ttu-id="e7d59-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7d59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7d59-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7d59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7d59-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7d59-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7d59-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7d59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7d59-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7d59-116">Not supported.</span></span>|
|<span data-ttu-id="e7d59-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7d59-117">Application</span></span>|<span data-ttu-id="e7d59-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7d59-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7d59-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7d59-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7d59-120">Optional query parameters</span></span>
<span data-ttu-id="e7d59-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d59-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e7d59-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d59-122">Request headers</span></span>
|<span data-ttu-id="e7d59-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7d59-123">Header</span></span>|<span data-ttu-id="e7d59-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e7d59-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7d59-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7d59-125">Authorization</span></span>|<span data-ttu-id="e7d59-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7d59-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7d59-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e7d59-127">Accept</span></span>|<span data-ttu-id="e7d59-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e7d59-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7d59-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d59-129">Request body</span></span>
<span data-ttu-id="e7d59-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7d59-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7d59-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d59-131">Response</span></span>
<span data-ttu-id="e7d59-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d59-132">If successful, this method returns a `200 OK` response code and [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7d59-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7d59-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7d59-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d59-134">Request</span></span>
<span data-ttu-id="e7d59-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7d59-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

### <a name="response"></a><span data-ttu-id="e7d59-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d59-136">Response</span></span>
<span data-ttu-id="e7d59-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7d59-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "value": {
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
}
```





