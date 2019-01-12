---
title: Acessar targetedManagedAppConfiguration
description: Ler propriedades e relações do objeto targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4907f142cb7b4526d284952b84598206dd37550a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951471"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="6ca12-103">Acessar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ca12-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="6ca12-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6ca12-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ca12-105">Leia as propriedades e as relações do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ca12-105">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ca12-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ca12-106">Prerequisites</span></span>
<span data-ttu-id="6ca12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ca12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ca12-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ca12-109">Permission type</span></span>|<span data-ttu-id="6ca12-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ca12-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ca12-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ca12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ca12-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ca12-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6ca12-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ca12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ca12-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ca12-114">Not supported.</span></span>|
|<span data-ttu-id="6ca12-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ca12-115">Application</span></span>|<span data-ttu-id="6ca12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ca12-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ca12-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ca12-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ca12-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6ca12-118">Optional query parameters</span></span>
<span data-ttu-id="6ca12-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ca12-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6ca12-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ca12-120">Request headers</span></span>
|<span data-ttu-id="6ca12-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ca12-121">Header</span></span>|<span data-ttu-id="6ca12-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ca12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ca12-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ca12-123">Authorization</span></span>|<span data-ttu-id="6ca12-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ca12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ca12-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ca12-125">Accept</span></span>|<span data-ttu-id="6ca12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ca12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ca12-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ca12-127">Request body</span></span>
<span data-ttu-id="6ca12-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ca12-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ca12-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ca12-129">Response</span></span>
<span data-ttu-id="6ca12-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ca12-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ca12-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ca12-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ca12-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ca12-132">Request</span></span>
<span data-ttu-id="6ca12-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ca12-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6ca12-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ca12-134">Response</span></span>
<span data-ttu-id="6ca12-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ca12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



