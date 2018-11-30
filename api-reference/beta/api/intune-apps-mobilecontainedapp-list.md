---
title: Lista mobileContainedApps
description: Lista as propriedades e os relacionamentos dos objetos mobileContainedApp.
ms.openlocfilehash: 77f15813f2f6a7b15d365e93d48bd3c923d36354
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035561"
---
# <a name="list-mobilecontainedapps"></a><span data-ttu-id="46499-103">Lista mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="46499-103">List mobileContainedApps</span></span>

> <span data-ttu-id="46499-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46499-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46499-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46499-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46499-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="46499-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46499-107">Lista as propriedades e os relacionamentos dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="46499-107">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46499-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46499-108">Prerequisites</span></span>
<span data-ttu-id="46499-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46499-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46499-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46499-111">Permission type</span></span>|<span data-ttu-id="46499-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46499-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46499-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46499-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46499-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="46499-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="46499-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46499-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46499-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46499-116">Not supported.</span></span>|
|<span data-ttu-id="46499-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46499-117">Application</span></span>|<span data-ttu-id="46499-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46499-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46499-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46499-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="46499-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46499-120">Request headers</span></span>
|<span data-ttu-id="46499-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46499-121">Header</span></span>|<span data-ttu-id="46499-122">Valor</span><span class="sxs-lookup"><span data-stu-id="46499-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46499-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="46499-123">Authorization</span></span>|<span data-ttu-id="46499-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46499-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46499-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46499-125">Accept</span></span>|<span data-ttu-id="46499-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46499-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46499-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46499-127">Request body</span></span>
<span data-ttu-id="46499-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46499-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46499-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="46499-129">Response</span></span>
<span data-ttu-id="46499-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46499-130">If successful, this method returns a `200 OK` response code and a collection of [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46499-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46499-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="46499-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46499-132">Request</span></span>
<span data-ttu-id="46499-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46499-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="46499-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="46499-134">Response</span></span>
<span data-ttu-id="46499-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46499-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 150

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileContainedApp",
      "id": "3c02d875-d875-3c02-75d8-023c75d8023c"
    }
  ]
}
```





