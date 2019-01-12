---
title: Acessar windows10CustomConfiguration
description: Leia as propriedades e as relações do objeto windows10CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6b083256f9bc755d41ac093ffdb84bf50de6f7c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925424"
---
# <a name="get-windows10customconfiguration"></a><span data-ttu-id="daaab-103">Acessar windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="daaab-103">Get windows10CustomConfiguration</span></span>

> <span data-ttu-id="daaab-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="daaab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="daaab-105">Leia as propriedades e as relações do objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="daaab-105">Read properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="daaab-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="daaab-106">Prerequisites</span></span>
<span data-ttu-id="daaab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daaab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daaab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daaab-109">Permission type</span></span>|<span data-ttu-id="daaab-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="daaab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daaab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daaab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="daaab-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="daaab-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="daaab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="daaab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daaab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daaab-114">Not supported.</span></span>|
|<span data-ttu-id="daaab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daaab-115">Application</span></span>|<span data-ttu-id="daaab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daaab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="daaab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daaab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="daaab-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="daaab-118">Optional query parameters</span></span>
<span data-ttu-id="daaab-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="daaab-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="daaab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daaab-120">Request headers</span></span>
|<span data-ttu-id="daaab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="daaab-121">Header</span></span>|<span data-ttu-id="daaab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="daaab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daaab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="daaab-123">Authorization</span></span>|<span data-ttu-id="daaab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daaab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daaab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="daaab-125">Accept</span></span>|<span data-ttu-id="daaab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="daaab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daaab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daaab-127">Request body</span></span>
<span data-ttu-id="daaab-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="daaab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daaab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="daaab-129">Response</span></span>
<span data-ttu-id="daaab-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daaab-130">If successful, this method returns a `200 OK` response code and [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daaab-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="daaab-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="daaab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daaab-132">Request</span></span>
<span data-ttu-id="daaab-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="daaab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="daaab-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="daaab-134">Response</span></span>
<span data-ttu-id="daaab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="daaab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
    "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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



