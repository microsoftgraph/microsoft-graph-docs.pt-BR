---
title: Obter mobileAppDependency
description: Leia as propriedades e as relações do objeto mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1256ea858627ca808446c389b08c9b8ed677b540
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155325"
---
# <a name="get-mobileappdependency"></a><span data-ttu-id="1d613-103">Obter mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="1d613-103">Get mobileAppDependency</span></span>

<span data-ttu-id="1d613-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d613-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d613-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d613-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d613-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d613-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d613-107">Leia as propriedades e as relações do [objeto mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="1d613-107">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d613-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d613-108">Prerequisites</span></span>
<span data-ttu-id="1d613-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d613-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d613-111">Permission type</span></span>|<span data-ttu-id="1d613-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d613-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d613-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d613-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d613-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d613-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1d613-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d613-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d613-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d613-116">Not supported.</span></span>|
|<span data-ttu-id="1d613-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d613-117">Application</span></span>|<span data-ttu-id="1d613-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d613-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d613-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d613-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d613-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1d613-120">Optional query parameters</span></span>
<span data-ttu-id="1d613-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1d613-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d613-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d613-122">Request headers</span></span>
|<span data-ttu-id="1d613-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d613-123">Header</span></span>|<span data-ttu-id="1d613-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1d613-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d613-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d613-125">Authorization</span></span>|<span data-ttu-id="1d613-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d613-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d613-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d613-127">Accept</span></span>|<span data-ttu-id="1d613-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1d613-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d613-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d613-129">Request body</span></span>
<span data-ttu-id="1d613-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d613-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d613-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d613-131">Response</span></span>
<span data-ttu-id="1d613-132">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d613-132">If successful, this method returns a `200 OK` response code and [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d613-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d613-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d613-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d613-134">Request</span></span>
<span data-ttu-id="1d613-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d613-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

### <a name="response"></a><span data-ttu-id="1d613-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d613-136">Response</span></span>
<span data-ttu-id="1d613-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d613-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppDependency",
    "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
    "targetId": "Target Id value",
    "targetDisplayName": "Target Display Name value",
    "targetDisplayVersion": "Target Display Version value",
    "targetPublisher": "Target Publisher value",
    "targetType": "parent",
    "dependencyType": "autoInstall",
    "dependentAppCount": 1,
    "dependsOnAppCount": 1
  }
}
```




