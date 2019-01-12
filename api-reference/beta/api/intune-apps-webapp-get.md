---
title: Acessar webApp
description: Leia as propriedades e as relações do objeto webApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b7cbf3b26099e0cd34b1fff342b10122e684b150
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990198"
---
# <a name="get-webapp"></a><span data-ttu-id="bc8eb-103">Acessar webApp</span><span class="sxs-lookup"><span data-stu-id="bc8eb-103">Get webApp</span></span>

> <span data-ttu-id="bc8eb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc8eb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc8eb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc8eb-107">Leia as propriedades e as relações do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc8eb-107">Read properties and relationships of the [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc8eb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc8eb-108">Prerequisites</span></span>
<span data-ttu-id="bc8eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc8eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc8eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc8eb-111">Permission type</span></span>|<span data-ttu-id="bc8eb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc8eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc8eb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc8eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc8eb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc8eb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bc8eb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc8eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc8eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-116">Not supported.</span></span>|
|<span data-ttu-id="bc8eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc8eb-117">Application</span></span>|<span data-ttu-id="bc8eb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc8eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc8eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc8eb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bc8eb-120">Optional query parameters</span></span>
<span data-ttu-id="bc8eb-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bc8eb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc8eb-122">Request headers</span></span>
|<span data-ttu-id="bc8eb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc8eb-123">Header</span></span>|<span data-ttu-id="bc8eb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="bc8eb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc8eb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc8eb-125">Authorization</span></span>|<span data-ttu-id="bc8eb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc8eb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc8eb-127">Accept</span></span>|<span data-ttu-id="bc8eb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bc8eb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc8eb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc8eb-129">Request body</span></span>
<span data-ttu-id="bc8eb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc8eb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc8eb-131">Response</span></span>
<span data-ttu-id="bc8eb-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-132">If successful, this method returns a `200 OK` response code and [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc8eb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc8eb-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc8eb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc8eb-134">Request</span></span>
<span data-ttu-id="bc8eb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="bc8eb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc8eb-136">Response</span></span>
<span data-ttu-id="bc8eb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc8eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 902

{
  "value": {
    "@odata.type": "#microsoft.graph.webApp",
    "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "appUrl": "https://example.com/appUrl/",
    "useManagedBrowser": true
  }
}
```





