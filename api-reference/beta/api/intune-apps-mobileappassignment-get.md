---
title: Acessar mobileAppAssignment
description: Leia as propriedades e as relações do objeto mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a91cf6ddd4ba47ad99eb2a3ae9723eec8b77aa0c
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177944"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="d6cce-103">Acessar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="d6cce-103">Get mobileAppAssignment</span></span>

<span data-ttu-id="d6cce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6cce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6cce-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6cce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6cce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6cce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6cce-107">Leia as propriedades e as relações do objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d6cce-107">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6cce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6cce-108">Prerequisites</span></span>
<span data-ttu-id="d6cce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6cce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6cce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6cce-111">Permission type</span></span>|<span data-ttu-id="d6cce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6cce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6cce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6cce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6cce-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6cce-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d6cce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6cce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6cce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6cce-116">Not supported.</span></span>|
|<span data-ttu-id="d6cce-117">Application</span><span class="sxs-lookup"><span data-stu-id="d6cce-117">Application</span></span>|<span data-ttu-id="d6cce-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6cce-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6cce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6cce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6cce-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d6cce-120">Optional query parameters</span></span>
<span data-ttu-id="d6cce-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d6cce-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6cce-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6cce-122">Request headers</span></span>
|<span data-ttu-id="d6cce-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6cce-123">Header</span></span>|<span data-ttu-id="d6cce-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d6cce-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6cce-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6cce-125">Authorization</span></span>|<span data-ttu-id="d6cce-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6cce-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6cce-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6cce-127">Accept</span></span>|<span data-ttu-id="d6cce-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d6cce-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6cce-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6cce-129">Request body</span></span>
<span data-ttu-id="d6cce-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6cce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6cce-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6cce-131">Response</span></span>
<span data-ttu-id="d6cce-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6cce-132">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6cce-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6cce-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6cce-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6cce-134">Request</span></span>
<span data-ttu-id="d6cce-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6cce-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d6cce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6cce-136">Response</span></span>
<span data-ttu-id="d6cce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6cce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppAssignment",
    "id": "591620b7-20b7-5916-b720-1659b7201659",
    "intent": "required",
    "target": {
      "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
    },
    "settings": {
      "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
      "vpnConfigurationId": "Vpn Configuration Id value",
      "uninstallOnDeviceRemoval": true
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```



