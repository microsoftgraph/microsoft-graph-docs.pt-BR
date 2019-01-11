---
title: Lista iosLobAppProvisioningConfigurations
description: Lista as propriedades e os relacionamentos dos objetos iosLobAppProvisioningConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8c61c5eba8b9bdb9654d573fbdf90e20bd8ff7cf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892453"
---
# <a name="list-ioslobappprovisioningconfigurations"></a><span data-ttu-id="f3059-103">Lista iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="f3059-103">List iosLobAppProvisioningConfigurations</span></span>

> <span data-ttu-id="f3059-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f3059-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3059-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f3059-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3059-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f3059-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3059-107">Lista as propriedades e os relacionamentos dos objetos [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f3059-107">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3059-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3059-108">Prerequisites</span></span>
<span data-ttu-id="f3059-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3059-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3059-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3059-111">Permission type</span></span>|<span data-ttu-id="f3059-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3059-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3059-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3059-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3059-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3059-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f3059-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3059-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3059-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3059-116">Not supported.</span></span>|
|<span data-ttu-id="f3059-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3059-117">Application</span></span>|<span data-ttu-id="f3059-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3059-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3059-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3059-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f3059-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3059-120">Request headers</span></span>
|<span data-ttu-id="f3059-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3059-121">Header</span></span>|<span data-ttu-id="f3059-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f3059-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3059-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3059-123">Authorization</span></span>|<span data-ttu-id="f3059-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3059-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3059-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3059-125">Accept</span></span>|<span data-ttu-id="f3059-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3059-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3059-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3059-127">Request body</span></span>
<span data-ttu-id="f3059-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3059-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3059-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3059-129">Response</span></span>
<span data-ttu-id="f3059-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3059-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3059-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3059-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3059-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3059-132">Request</span></span>
<span data-ttu-id="f3059-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3059-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
```

### <a name="response"></a><span data-ttu-id="f3059-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3059-134">Response</span></span>
<span data-ttu-id="f3059-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3059-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
      "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```





