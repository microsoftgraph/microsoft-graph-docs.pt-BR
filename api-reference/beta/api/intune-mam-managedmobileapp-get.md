---
title: Acessar managedMobileApp
description: Leia as propriedades e as relações do objeto managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc466a65e4a345697595ae62897fd9c118ed4b02
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157873"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="96b58-103">Acessar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="96b58-103">Get managedMobileApp</span></span>

<span data-ttu-id="96b58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96b58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96b58-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96b58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96b58-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96b58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96b58-107">Leia as propriedades e as relações do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96b58-107">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96b58-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96b58-108">Prerequisites</span></span>
<span data-ttu-id="96b58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96b58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96b58-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96b58-111">Permission type</span></span>|<span data-ttu-id="96b58-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96b58-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96b58-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96b58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96b58-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96b58-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="96b58-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96b58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96b58-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96b58-116">Not supported.</span></span>|
|<span data-ttu-id="96b58-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96b58-117">Application</span></span>|<span data-ttu-id="96b58-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96b58-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96b58-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96b58-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="96b58-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="96b58-120">Optional query parameters</span></span>
<span data-ttu-id="96b58-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="96b58-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96b58-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96b58-122">Request headers</span></span>
|<span data-ttu-id="96b58-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96b58-123">Header</span></span>|<span data-ttu-id="96b58-124">Valor</span><span class="sxs-lookup"><span data-stu-id="96b58-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96b58-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="96b58-125">Authorization</span></span>|<span data-ttu-id="96b58-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96b58-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96b58-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96b58-127">Accept</span></span>|<span data-ttu-id="96b58-128">application/json</span><span class="sxs-lookup"><span data-stu-id="96b58-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96b58-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96b58-129">Request body</span></span>
<span data-ttu-id="96b58-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96b58-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96b58-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="96b58-131">Response</span></span>
<span data-ttu-id="96b58-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96b58-132">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96b58-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96b58-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="96b58-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96b58-134">Request</span></span>
<span data-ttu-id="96b58-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96b58-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="96b58-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="96b58-136">Response</span></span>
<span data-ttu-id="96b58-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96b58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 309

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileApp",
    "mobileAppIdentifier": {
      "@odata.type": "microsoft.graph.windowsAppIdentifier",
      "windowsAppId": "Windows App Id value"
    },
    "id": "0a129715-9715-0a12-1597-120a1597120a",
    "version": "Version value"
  }
}
```




