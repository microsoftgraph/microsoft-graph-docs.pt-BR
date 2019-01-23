---
title: Lista windowsUniversalAppXContainedApps
description: Lista as propriedades e os relacionamentos dos objetos windowsUniversalAppXContainedApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d2376074a3e6ce46b8e042c181fe7df0a9d9cf4b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417809"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="17f53-103">Lista windowsUniversalAppXContainedApps</span><span class="sxs-lookup"><span data-stu-id="17f53-103">List windowsUniversalAppXContainedApps</span></span>

> <span data-ttu-id="17f53-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="17f53-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="17f53-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17f53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17f53-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="17f53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17f53-107">Lista as propriedades e os relacionamentos dos objetos [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="17f53-107">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17f53-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17f53-108">Prerequisites</span></span>
<span data-ttu-id="17f53-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="17f53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="17f53-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17f53-111">Permission type</span></span>|<span data-ttu-id="17f53-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17f53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17f53-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17f53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17f53-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="17f53-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="17f53-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17f53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17f53-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17f53-116">Not supported.</span></span>|
|<span data-ttu-id="17f53-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17f53-117">Application</span></span>|<span data-ttu-id="17f53-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17f53-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17f53-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17f53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="17f53-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17f53-120">Request headers</span></span>
|<span data-ttu-id="17f53-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17f53-121">Header</span></span>|<span data-ttu-id="17f53-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17f53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17f53-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17f53-123">Authorization</span></span>|<span data-ttu-id="17f53-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17f53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17f53-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17f53-125">Accept</span></span>|<span data-ttu-id="17f53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17f53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17f53-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17f53-127">Request body</span></span>
<span data-ttu-id="17f53-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17f53-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17f53-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="17f53-129">Response</span></span>
<span data-ttu-id="17f53-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17f53-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17f53-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17f53-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="17f53-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17f53-132">Request</span></span>
<span data-ttu-id="17f53-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17f53-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="17f53-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="17f53-134">Response</span></span>
<span data-ttu-id="17f53-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17f53-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
      "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
      "appUserModelId": "App User Model Id value"
    }
  ]
}
```




