---
title: Obter androidWorkProfileCustomConfiguration
description: Leia as propriedades e os relacionamentos do objeto androidWorkProfileCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 4e12962e59bc45635b202aeda08e7e8c299bc51c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328564"
---
# <a name="get-androidworkprofilecustomconfiguration"></a><span data-ttu-id="578ef-103">Obter androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="578ef-103">Get androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="578ef-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="578ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="578ef-105">Leia as propriedades e os relacionamentos do objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="578ef-105">Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="578ef-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="578ef-106">Prerequisites</span></span>
<span data-ttu-id="578ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="578ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="578ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="578ef-109">Permission type</span></span>|<span data-ttu-id="578ef-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="578ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="578ef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="578ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="578ef-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="578ef-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="578ef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="578ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="578ef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="578ef-114">Not supported.</span></span>|
|<span data-ttu-id="578ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="578ef-115">Application</span></span>|<span data-ttu-id="578ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="578ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="578ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="578ef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="578ef-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="578ef-118">Optional query parameters</span></span>
<span data-ttu-id="578ef-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="578ef-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="578ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="578ef-120">Request headers</span></span>
|<span data-ttu-id="578ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="578ef-121">Header</span></span>|<span data-ttu-id="578ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="578ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="578ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="578ef-123">Authorization</span></span>|<span data-ttu-id="578ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="578ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="578ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="578ef-125">Accept</span></span>|<span data-ttu-id="578ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="578ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="578ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="578ef-127">Request body</span></span>
<span data-ttu-id="578ef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="578ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="578ef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="578ef-129">Response</span></span>
<span data-ttu-id="578ef-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="578ef-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="578ef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="578ef-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="578ef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="578ef-132">Request</span></span>
<span data-ttu-id="578ef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="578ef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="578ef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="578ef-134">Response</span></span>
<span data-ttu-id="578ef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="578ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 636

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
    "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```



