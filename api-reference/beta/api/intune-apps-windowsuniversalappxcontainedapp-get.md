---
title: Obter windowsUniversalAppXContainedApp
description: Leia as propriedades e as relações do objeto windowsUniversalAppXContainedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e4d2832833573634d243aa5a3188204bedb7eaa
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39932359"
---
# <a name="get-windowsuniversalappxcontainedapp"></a><span data-ttu-id="5c100-103">Obter windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="5c100-103">Get windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="5c100-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c100-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c100-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c100-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c100-106">Leia as propriedades e as relações do objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="5c100-106">Read properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c100-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c100-107">Prerequisites</span></span>
<span data-ttu-id="5c100-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c100-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c100-110">Permission type</span></span>|<span data-ttu-id="5c100-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c100-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c100-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c100-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c100-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c100-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5c100-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c100-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c100-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c100-115">Not supported.</span></span>|
|<span data-ttu-id="5c100-116">Application</span><span class="sxs-lookup"><span data-stu-id="5c100-116">Application</span></span>|<span data-ttu-id="5c100-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c100-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c100-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c100-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c100-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c100-119">Optional query parameters</span></span>
<span data-ttu-id="5c100-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c100-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c100-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c100-121">Request headers</span></span>
|<span data-ttu-id="5c100-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c100-122">Header</span></span>|<span data-ttu-id="5c100-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5c100-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c100-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c100-124">Authorization</span></span>|<span data-ttu-id="5c100-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c100-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c100-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c100-126">Accept</span></span>|<span data-ttu-id="5c100-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5c100-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c100-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c100-128">Request body</span></span>
<span data-ttu-id="5c100-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c100-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c100-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c100-130">Response</span></span>
<span data-ttu-id="5c100-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c100-131">If successful, this method returns a `200 OK` response code and [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c100-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c100-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c100-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c100-133">Request</span></span>
<span data-ttu-id="5c100-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c100-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="5c100-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c100-135">Response</span></span>
<span data-ttu-id="5c100-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c100-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
    "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
    "appUserModelId": "App User Model Id value"
  }
}
```





