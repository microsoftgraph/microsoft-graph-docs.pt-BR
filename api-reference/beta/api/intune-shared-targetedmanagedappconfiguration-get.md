---
title: Acessar targetedManagedAppConfiguration
description: Leia as propriedades e as relações do objeto targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ce0d053618597e1ff678f4b5daa51fc023a420b9
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085630"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="bd670-103">Acessar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd670-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="bd670-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bd670-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd670-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd670-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd670-106">Leia as propriedades e as relações do objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd670-106">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd670-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd670-107">Prerequisites</span></span>
<span data-ttu-id="bd670-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd670-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd670-110">Permission type</span></span>|<span data-ttu-id="bd670-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bd670-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd670-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd670-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bd670-113">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="bd670-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="bd670-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd670-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="bd670-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="bd670-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="bd670-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd670-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bd670-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd670-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd670-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd670-118">Not supported.</span></span>|
|<span data-ttu-id="bd670-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd670-119">Application</span></span>||
| <span data-ttu-id="bd670-120">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="bd670-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="bd670-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd670-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="bd670-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="bd670-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="bd670-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd670-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd670-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd670-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd670-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd670-125">Optional query parameters</span></span>
<span data-ttu-id="bd670-126">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bd670-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd670-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd670-127">Request headers</span></span>
|<span data-ttu-id="bd670-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd670-128">Header</span></span>|<span data-ttu-id="bd670-129">Valor</span><span class="sxs-lookup"><span data-stu-id="bd670-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd670-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd670-130">Authorization</span></span>|<span data-ttu-id="bd670-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd670-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd670-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bd670-132">Accept</span></span>|<span data-ttu-id="bd670-133">application/json</span><span class="sxs-lookup"><span data-stu-id="bd670-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd670-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd670-134">Request body</span></span>
<span data-ttu-id="bd670-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd670-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd670-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd670-136">Response</span></span>
<span data-ttu-id="bd670-137">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd670-137">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd670-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd670-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd670-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd670-139">Request</span></span>
<span data-ttu-id="bd670-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd670-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bd670-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd670-141">Response</span></span>
<span data-ttu-id="bd670-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd670-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









