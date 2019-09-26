---
title: Acessar targetedManagedAppConfiguration
description: Leia as propriedades e as relações do objeto targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6f7d48e88779d31f348ba561e2c10b4a21094da2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199534"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="c8148-103">Acessar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8148-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="c8148-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8148-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8148-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8148-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8148-106">Leia as propriedades e as relações do objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8148-106">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8148-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8148-107">Prerequisites</span></span>
<span data-ttu-id="c8148-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8148-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8148-110">Permission type</span></span>|<span data-ttu-id="c8148-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8148-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8148-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8148-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c8148-113">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="c8148-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c8148-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8148-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c8148-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c8148-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c8148-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8148-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c8148-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8148-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8148-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8148-118">Not supported.</span></span>|
|<span data-ttu-id="c8148-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8148-119">Application</span></span>||
| <span data-ttu-id="c8148-120">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="c8148-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c8148-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8148-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c8148-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c8148-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c8148-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8148-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8148-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8148-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8148-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c8148-125">Optional query parameters</span></span>
<span data-ttu-id="c8148-126">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c8148-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8148-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8148-127">Request headers</span></span>
|<span data-ttu-id="c8148-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8148-128">Header</span></span>|<span data-ttu-id="c8148-129">Valor</span><span class="sxs-lookup"><span data-stu-id="c8148-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8148-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8148-130">Authorization</span></span>|<span data-ttu-id="c8148-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8148-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8148-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8148-132">Accept</span></span>|<span data-ttu-id="c8148-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c8148-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8148-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8148-134">Request body</span></span>
<span data-ttu-id="c8148-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8148-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8148-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8148-136">Response</span></span>
<span data-ttu-id="c8148-137">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8148-137">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8148-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8148-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8148-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8148-139">Request</span></span>
<span data-ttu-id="c8148-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8148-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c8148-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8148-141">Response</span></span>
<span data-ttu-id="c8148-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8148-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 679

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2444e029-e029-2444-29e0-442429e04424",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```




