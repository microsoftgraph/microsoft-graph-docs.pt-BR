---
title: Obter deviceManagementAbstractComplexSettingInstance
description: Leia as propriedades e as relações do objeto deviceManagementAbstractComplexSettingInstance.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04e9572f32ffcc6ffae226577bfdfa58ffb03f49
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522759"
---
# <a name="get-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="99801-103">Obter deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="99801-103">Get deviceManagementAbstractComplexSettingInstance</span></span>

> <span data-ttu-id="99801-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99801-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99801-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99801-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99801-106">Leia as propriedades e as relações do objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="99801-106">Read properties and relationships of the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99801-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99801-107">Prerequisites</span></span>
<span data-ttu-id="99801-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99801-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99801-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99801-110">Permission type</span></span>|<span data-ttu-id="99801-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99801-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99801-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99801-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99801-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="99801-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="99801-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99801-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99801-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99801-115">Not supported.</span></span>|
|<span data-ttu-id="99801-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99801-116">Application</span></span>|<span data-ttu-id="99801-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99801-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99801-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99801-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99801-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99801-119">Optional query parameters</span></span>
<span data-ttu-id="99801-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="99801-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99801-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99801-121">Request headers</span></span>
|<span data-ttu-id="99801-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99801-122">Header</span></span>|<span data-ttu-id="99801-123">Valor</span><span class="sxs-lookup"><span data-stu-id="99801-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99801-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="99801-124">Authorization</span></span>|<span data-ttu-id="99801-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99801-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99801-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99801-126">Accept</span></span>|<span data-ttu-id="99801-127">application/json</span><span class="sxs-lookup"><span data-stu-id="99801-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99801-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99801-128">Request body</span></span>
<span data-ttu-id="99801-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99801-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99801-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="99801-130">Response</span></span>
<span data-ttu-id="99801-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99801-131">If successful, this method returns a `200 OK` response code and [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99801-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99801-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="99801-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99801-133">Request</span></span>
<span data-ttu-id="99801-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99801-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="99801-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="99801-135">Response</span></span>
<span data-ttu-id="99801-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99801-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
    "id": "433e9565-9565-433e-6595-3e4365953e43",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value",
    "implementationId": "Implementation Id value"
  }
}
```







