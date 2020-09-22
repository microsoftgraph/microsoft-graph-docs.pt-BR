---
title: Acessar targetedManagedAppConfiguration
description: Leia as propriedades e as relações do objeto targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a6fca0c311362ad9ba66242b7b2465cfbc06b64f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999801"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="904db-103">Acessar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="904db-103">Get targetedManagedAppConfiguration</span></span>

<span data-ttu-id="904db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="904db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="904db-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="904db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="904db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="904db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="904db-107">Leia as propriedades e as relações do objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="904db-107">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="904db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="904db-108">Prerequisites</span></span>
<span data-ttu-id="904db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="904db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="904db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="904db-111">Permission type</span></span>|<span data-ttu-id="904db-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="904db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="904db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="904db-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="904db-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="904db-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="904db-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="904db-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="904db-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="904db-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="904db-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="904db-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="904db-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="904db-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="904db-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="904db-119">Not supported.</span></span>|
|<span data-ttu-id="904db-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="904db-120">Application</span></span>||
| <span data-ttu-id="904db-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="904db-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="904db-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="904db-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="904db-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="904db-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="904db-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="904db-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="904db-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="904db-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="904db-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="904db-126">Optional query parameters</span></span>
<span data-ttu-id="904db-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="904db-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="904db-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="904db-128">Request headers</span></span>
|<span data-ttu-id="904db-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="904db-129">Header</span></span>|<span data-ttu-id="904db-130">Valor</span><span class="sxs-lookup"><span data-stu-id="904db-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="904db-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="904db-131">Authorization</span></span>|<span data-ttu-id="904db-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="904db-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="904db-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="904db-133">Accept</span></span>|<span data-ttu-id="904db-134">application/json</span><span class="sxs-lookup"><span data-stu-id="904db-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="904db-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="904db-135">Request body</span></span>
<span data-ttu-id="904db-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="904db-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="904db-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="904db-137">Response</span></span>
<span data-ttu-id="904db-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="904db-138">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="904db-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="904db-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="904db-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="904db-140">Request</span></span>
<span data-ttu-id="904db-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="904db-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="904db-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="904db-142">Response</span></span>
<span data-ttu-id="904db-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="904db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









