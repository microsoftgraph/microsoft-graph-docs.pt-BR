---
title: Acessar managedMobileApp
description: Leia as propriedades e as relações do objeto managedMobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3662efdfe7d675cd7d256c9fb7c1fcbbd49c4cf8
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086792"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="3ee34-103">Acessar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="3ee34-103">Get managedMobileApp</span></span>

> <span data-ttu-id="3ee34-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ee34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ee34-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ee34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ee34-106">Leia as propriedades e as relações do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ee34-106">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ee34-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ee34-107">Prerequisites</span></span>
<span data-ttu-id="3ee34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ee34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ee34-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ee34-110">Permission type</span></span>|<span data-ttu-id="3ee34-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3ee34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ee34-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ee34-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ee34-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ee34-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3ee34-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ee34-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ee34-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ee34-115">Not supported.</span></span>|
|<span data-ttu-id="3ee34-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ee34-116">Application</span></span>|<span data-ttu-id="3ee34-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ee34-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ee34-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ee34-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ee34-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3ee34-119">Optional query parameters</span></span>
<span data-ttu-id="3ee34-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3ee34-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ee34-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee34-121">Request headers</span></span>
|<span data-ttu-id="3ee34-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ee34-122">Header</span></span>|<span data-ttu-id="3ee34-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3ee34-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ee34-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ee34-124">Authorization</span></span>|<span data-ttu-id="3ee34-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ee34-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ee34-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ee34-126">Accept</span></span>|<span data-ttu-id="3ee34-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3ee34-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ee34-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee34-128">Request body</span></span>
<span data-ttu-id="3ee34-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ee34-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ee34-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ee34-130">Response</span></span>
<span data-ttu-id="3ee34-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ee34-131">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ee34-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ee34-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ee34-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee34-133">Request</span></span>
<span data-ttu-id="3ee34-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ee34-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="3ee34-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ee34-135">Response</span></span>
<span data-ttu-id="3ee34-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ee34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileApp",
    "mobileAppIdentifier": {
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "0a129715-9715-0a12-1597-120a1597120a",
    "version": "Version value"
  }
}
```






