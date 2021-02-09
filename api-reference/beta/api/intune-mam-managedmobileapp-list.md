---
title: Listar managedMobileApps
description: Listar propriedades e relações dos objetos managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5483b049e86f68a958f4dcf64e574a7753c61d40
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157859"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="37030-103">Listar managedMobileApps</span><span class="sxs-lookup"><span data-stu-id="37030-103">List managedMobileApps</span></span>

<span data-ttu-id="37030-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37030-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37030-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37030-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37030-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37030-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37030-107">Listar propriedades e relações dos objetos [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37030-107">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37030-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37030-108">Prerequisites</span></span>
<span data-ttu-id="37030-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37030-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37030-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37030-111">Permission type</span></span>|<span data-ttu-id="37030-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37030-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37030-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37030-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37030-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="37030-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="37030-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37030-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37030-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37030-116">Not supported.</span></span>|
|<span data-ttu-id="37030-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37030-117">Application</span></span>|<span data-ttu-id="37030-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="37030-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37030-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37030-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="37030-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37030-120">Request headers</span></span>
|<span data-ttu-id="37030-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37030-121">Header</span></span>|<span data-ttu-id="37030-122">Valor</span><span class="sxs-lookup"><span data-stu-id="37030-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37030-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="37030-123">Authorization</span></span>|<span data-ttu-id="37030-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37030-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37030-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37030-125">Accept</span></span>|<span data-ttu-id="37030-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37030-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37030-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37030-127">Request body</span></span>
<span data-ttu-id="37030-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37030-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37030-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="37030-129">Response</span></span>
<span data-ttu-id="37030-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37030-130">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37030-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37030-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="37030-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37030-132">Request</span></span>
<span data-ttu-id="37030-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37030-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="37030-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="37030-134">Response</span></span>
<span data-ttu-id="37030-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37030-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 337

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```




