---
title: Obter windowsUniversalAppXContainedApp
description: Leia as propriedades e as relações do objeto windowsUniversalAppXContainedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69156cb807a5431646ec7745ab4ae931522d37d6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706832"
---
# <a name="get-windowsuniversalappxcontainedapp"></a><span data-ttu-id="4accf-103">Obter windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="4accf-103">Get windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="4accf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4accf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4accf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4accf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4accf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4accf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4accf-107">Leia as propriedades e as relações do objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="4accf-107">Read properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4accf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4accf-108">Prerequisites</span></span>
<span data-ttu-id="4accf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4accf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4accf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4accf-111">Permission type</span></span>|<span data-ttu-id="4accf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4accf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4accf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4accf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4accf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4accf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4accf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4accf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4accf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4accf-116">Not supported.</span></span>|
|<span data-ttu-id="4accf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4accf-117">Application</span></span>|<span data-ttu-id="4accf-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4accf-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4accf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4accf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4accf-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4accf-120">Optional query parameters</span></span>
<span data-ttu-id="4accf-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4accf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4accf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4accf-122">Request headers</span></span>
|<span data-ttu-id="4accf-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4accf-123">Header</span></span>|<span data-ttu-id="4accf-124">Valor</span><span class="sxs-lookup"><span data-stu-id="4accf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4accf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4accf-125">Authorization</span></span>|<span data-ttu-id="4accf-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4accf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4accf-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4accf-127">Accept</span></span>|<span data-ttu-id="4accf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4accf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4accf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4accf-129">Request body</span></span>
<span data-ttu-id="4accf-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4accf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4accf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4accf-131">Response</span></span>
<span data-ttu-id="4accf-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4accf-132">If successful, this method returns a `200 OK` response code and [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4accf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4accf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4accf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4accf-134">Request</span></span>
<span data-ttu-id="4accf-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4accf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="4accf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4accf-136">Response</span></span>
<span data-ttu-id="4accf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4accf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





