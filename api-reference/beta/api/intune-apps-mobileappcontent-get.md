---
title: Acessar mobileAppContent
description: Leia as propriedades e as relações do objeto mobileAppContent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 96863a8e3de9f6a24ace8e58268a589897105e8e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39935628"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="62640-103">Acessar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="62640-103">Get mobileAppContent</span></span>

> <span data-ttu-id="62640-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62640-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62640-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62640-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62640-106">Leia as propriedades e as relações do objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="62640-106">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62640-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62640-107">Prerequisites</span></span>
<span data-ttu-id="62640-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62640-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62640-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62640-110">Permission type</span></span>|<span data-ttu-id="62640-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62640-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62640-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62640-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62640-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="62640-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="62640-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62640-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62640-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62640-115">Not supported.</span></span>|
|<span data-ttu-id="62640-116">Application</span><span class="sxs-lookup"><span data-stu-id="62640-116">Application</span></span>|<span data-ttu-id="62640-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="62640-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62640-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62640-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62640-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="62640-119">Optional query parameters</span></span>
<span data-ttu-id="62640-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="62640-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62640-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62640-121">Request headers</span></span>
|<span data-ttu-id="62640-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62640-122">Header</span></span>|<span data-ttu-id="62640-123">Valor</span><span class="sxs-lookup"><span data-stu-id="62640-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62640-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="62640-124">Authorization</span></span>|<span data-ttu-id="62640-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62640-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62640-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62640-126">Accept</span></span>|<span data-ttu-id="62640-127">application/json</span><span class="sxs-lookup"><span data-stu-id="62640-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62640-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62640-128">Request body</span></span>
<span data-ttu-id="62640-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62640-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62640-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="62640-130">Response</span></span>
<span data-ttu-id="62640-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62640-131">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62640-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62640-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="62640-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62640-133">Request</span></span>
<span data-ttu-id="62640-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62640-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="62640-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="62640-135">Response</span></span>
<span data-ttu-id="62640-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62640-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContent",
    "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
  }
}
```





