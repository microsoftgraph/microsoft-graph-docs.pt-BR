---
title: Obter mobileAppDependency
description: Leia as propriedades e as relações do objeto mobileAppDependency.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94cacfff449e499b811932d39a2b63003dc668ac
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329142"
---
# <a name="get-mobileappdependency"></a><span data-ttu-id="96325-103">Obter mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="96325-103">Get mobileAppDependency</span></span>

> <span data-ttu-id="96325-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96325-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96325-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96325-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96325-106">Leia as propriedades e as relações do objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="96325-106">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96325-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96325-107">Prerequisites</span></span>
<span data-ttu-id="96325-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96325-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96325-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96325-110">Permission type</span></span>|<span data-ttu-id="96325-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96325-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96325-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96325-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96325-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96325-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="96325-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96325-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96325-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96325-115">Not supported.</span></span>|
|<span data-ttu-id="96325-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96325-116">Application</span></span>|<span data-ttu-id="96325-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96325-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96325-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96325-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96325-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="96325-119">Optional query parameters</span></span>
<span data-ttu-id="96325-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="96325-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96325-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96325-121">Request headers</span></span>
|<span data-ttu-id="96325-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96325-122">Header</span></span>|<span data-ttu-id="96325-123">Valor</span><span class="sxs-lookup"><span data-stu-id="96325-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96325-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="96325-124">Authorization</span></span>|<span data-ttu-id="96325-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96325-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96325-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96325-126">Accept</span></span>|<span data-ttu-id="96325-127">application/json</span><span class="sxs-lookup"><span data-stu-id="96325-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96325-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96325-128">Request body</span></span>
<span data-ttu-id="96325-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96325-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96325-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="96325-130">Response</span></span>
<span data-ttu-id="96325-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96325-131">If successful, this method returns a `200 OK` response code and [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96325-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96325-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="96325-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96325-133">Request</span></span>
<span data-ttu-id="96325-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96325-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

### <a name="response"></a><span data-ttu-id="96325-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="96325-135">Response</span></span>
<span data-ttu-id="96325-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96325-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppDependency",
    "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
    "targetId": "Target Id value",
    "targetDisplayName": "Target Display Name value",
    "dependencyType": "autoInstall",
    "dependentAppCount": 1
  }
}
```






