---
title: Lista windowsUniversalAppXContainedApps
description: Lista as propriedades e os relacionamentos dos objetos windowsUniversalAppXContainedApp.
author: tfitzmac
ms.openlocfilehash: f28efa8a32c45d297670789a7726319fd96cc0b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301978"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="fb5ef-103">Lista windowsUniversalAppXContainedApps</span><span class="sxs-lookup"><span data-stu-id="fb5ef-103">List windowsUniversalAppXContainedApps</span></span>

> <span data-ttu-id="fb5ef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb5ef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb5ef-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb5ef-107">Lista as propriedades e os relacionamentos dos objetos [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fb5ef-107">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb5ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb5ef-108">Prerequisites</span></span>
<span data-ttu-id="fb5ef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb5ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb5ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb5ef-111">Permission type</span></span>|<span data-ttu-id="fb5ef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb5ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb5ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb5ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb5ef-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb5ef-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fb5ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb5ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb5ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-116">Not supported.</span></span>|
|<span data-ttu-id="fb5ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb5ef-117">Application</span></span>|<span data-ttu-id="fb5ef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb5ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb5ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="fb5ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb5ef-120">Request headers</span></span>
|<span data-ttu-id="fb5ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb5ef-121">Header</span></span>|<span data-ttu-id="fb5ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fb5ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb5ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb5ef-123">Authorization</span></span>|<span data-ttu-id="fb5ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb5ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb5ef-125">Accept</span></span>|<span data-ttu-id="fb5ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb5ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb5ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb5ef-127">Request body</span></span>
<span data-ttu-id="fb5ef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb5ef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb5ef-129">Response</span></span>
<span data-ttu-id="fb5ef-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb5ef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb5ef-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb5ef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb5ef-132">Request</span></span>
<span data-ttu-id="fb5ef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="fb5ef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb5ef-134">Response</span></span>
<span data-ttu-id="fb5ef-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb5ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
      "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
      "appUserModelId": "App User Model Id value"
    }
  ]
}
```





