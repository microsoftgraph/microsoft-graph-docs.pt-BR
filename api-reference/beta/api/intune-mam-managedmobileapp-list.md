---
title: Listar managedMobileApps
description: Listar propriedades e relações dos objetos managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec832e0cccd27c1f3e159c53101fd62514c34e89
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150551"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="88aaa-103">Listar managedMobileApps</span><span class="sxs-lookup"><span data-stu-id="88aaa-103">List managedMobileApps</span></span>

> <span data-ttu-id="88aaa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88aaa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88aaa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88aaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88aaa-106">Listar propriedades e relações dos objetos [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="88aaa-106">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88aaa-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88aaa-107">Prerequisites</span></span>
<span data-ttu-id="88aaa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="88aaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88aaa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88aaa-110">Permission type</span></span>|<span data-ttu-id="88aaa-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88aaa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88aaa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88aaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88aaa-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88aaa-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="88aaa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88aaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88aaa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88aaa-115">Not supported.</span></span>|
|<span data-ttu-id="88aaa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88aaa-116">Application</span></span>|<span data-ttu-id="88aaa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88aaa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88aaa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88aaa-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="88aaa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88aaa-119">Request headers</span></span>
|<span data-ttu-id="88aaa-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88aaa-120">Header</span></span>|<span data-ttu-id="88aaa-121">Valor</span><span class="sxs-lookup"><span data-stu-id="88aaa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88aaa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="88aaa-122">Authorization</span></span>|<span data-ttu-id="88aaa-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88aaa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88aaa-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88aaa-124">Accept</span></span>|<span data-ttu-id="88aaa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88aaa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88aaa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88aaa-126">Request body</span></span>
<span data-ttu-id="88aaa-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88aaa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88aaa-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="88aaa-128">Response</span></span>
<span data-ttu-id="88aaa-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88aaa-129">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88aaa-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88aaa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="88aaa-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88aaa-131">Request</span></span>
<span data-ttu-id="88aaa-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88aaa-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="88aaa-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="88aaa-133">Response</span></span>
<span data-ttu-id="88aaa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88aaa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```




