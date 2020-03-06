---
title: Listar managedMobileApps
description: Listar propriedades e relações dos objetos managedMobileApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 277b360472d8cbd3952bb6749a8784c316d16e67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513032"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="236f4-103">Listar managedMobileApps</span><span class="sxs-lookup"><span data-stu-id="236f4-103">List managedMobileApps</span></span>

<span data-ttu-id="236f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="236f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="236f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="236f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="236f4-106">Listar propriedades e relações dos objetos [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="236f4-106">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="236f4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="236f4-107">Prerequisites</span></span>
<span data-ttu-id="236f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="236f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="236f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="236f4-110">Permission type</span></span>|<span data-ttu-id="236f4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="236f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="236f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="236f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="236f4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="236f4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="236f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="236f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="236f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="236f4-115">Not supported.</span></span>|
|<span data-ttu-id="236f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="236f4-116">Application</span></span>|<span data-ttu-id="236f4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="236f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="236f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="236f4-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="236f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="236f4-119">Request headers</span></span>
|<span data-ttu-id="236f4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="236f4-120">Header</span></span>|<span data-ttu-id="236f4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="236f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="236f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="236f4-122">Authorization</span></span>|<span data-ttu-id="236f4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="236f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="236f4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="236f4-124">Accept</span></span>|<span data-ttu-id="236f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="236f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="236f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="236f4-126">Request body</span></span>
<span data-ttu-id="236f4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="236f4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="236f4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="236f4-128">Response</span></span>
<span data-ttu-id="236f4-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="236f4-129">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="236f4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="236f4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="236f4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="236f4-131">Request</span></span>
<span data-ttu-id="236f4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="236f4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="236f4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="236f4-133">Response</span></span>
<span data-ttu-id="236f4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="236f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




