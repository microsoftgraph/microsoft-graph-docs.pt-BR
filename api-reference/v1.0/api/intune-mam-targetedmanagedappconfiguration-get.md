---
title: Acessar targetedManagedAppConfiguration
description: Ler propriedades e relações do objeto targetedManagedAppConfiguration.
author: tfitzmac
ms.openlocfilehash: f40ae61063967239642ba3cc16403b7fcb7b04e2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306710"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="f1746-103">Acessar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1746-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="f1746-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f1746-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1746-105">Leia as propriedades e as relações do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1746-105">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1746-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1746-106">Prerequisites</span></span>
<span data-ttu-id="f1746-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1746-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1746-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1746-109">Permission type</span></span>|<span data-ttu-id="f1746-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1746-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1746-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1746-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1746-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1746-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f1746-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1746-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1746-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1746-114">Not supported.</span></span>|
|<span data-ttu-id="f1746-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1746-115">Application</span></span>|<span data-ttu-id="f1746-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1746-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1746-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1746-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1746-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1746-118">Optional query parameters</span></span>
<span data-ttu-id="f1746-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1746-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1746-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1746-120">Request headers</span></span>
|<span data-ttu-id="f1746-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1746-121">Header</span></span>|<span data-ttu-id="f1746-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f1746-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1746-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1746-123">Authorization</span></span>|<span data-ttu-id="f1746-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1746-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1746-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1746-125">Accept</span></span>|<span data-ttu-id="f1746-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1746-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1746-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1746-127">Request body</span></span>
<span data-ttu-id="f1746-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1746-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1746-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1746-129">Response</span></span>
<span data-ttu-id="f1746-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1746-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1746-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1746-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1746-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1746-132">Request</span></span>
<span data-ttu-id="f1746-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1746-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f1746-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1746-134">Response</span></span>
<span data-ttu-id="f1746-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1746-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



