---
title: Obter deviceManagementBooleanSettingInstance
description: Leia as propriedades e as relações do objeto deviceManagementBooleanSettingInstance.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bcb8f382f0dd394d84456406de2f21ee16a7a1e0
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522745"
---
# <a name="get-devicemanagementbooleansettinginstance"></a><span data-ttu-id="4bc2c-103">Obter deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="4bc2c-103">Get deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="4bc2c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bc2c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bc2c-106">Leia as propriedades e as relações do objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="4bc2c-106">Read properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bc2c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4bc2c-107">Prerequisites</span></span>
<span data-ttu-id="4bc2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bc2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bc2c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bc2c-110">Permission type</span></span>|<span data-ttu-id="4bc2c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4bc2c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bc2c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bc2c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4bc2c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bc2c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4bc2c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bc2c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bc2c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-115">Not supported.</span></span>|
|<span data-ttu-id="4bc2c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bc2c-116">Application</span></span>|<span data-ttu-id="4bc2c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bc2c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bc2c-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="4bc2c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4bc2c-119">Optional query parameters</span></span>
<span data-ttu-id="4bc2c-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bc2c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc2c-121">Request headers</span></span>
|<span data-ttu-id="4bc2c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bc2c-122">Header</span></span>|<span data-ttu-id="4bc2c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4bc2c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bc2c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bc2c-124">Authorization</span></span>|<span data-ttu-id="4bc2c-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bc2c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4bc2c-126">Accept</span></span>|<span data-ttu-id="4bc2c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4bc2c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bc2c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc2c-128">Request body</span></span>
<span data-ttu-id="4bc2c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bc2c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bc2c-130">Response</span></span>
<span data-ttu-id="4bc2c-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-131">If successful, this method returns a `200 OK` response code and [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bc2c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bc2c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bc2c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc2c-133">Request</span></span>
<span data-ttu-id="4bc2c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="4bc2c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bc2c-135">Response</span></span>
<span data-ttu-id="4bc2c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bc2c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 254

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
    "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value",
    "value": true
  }
}
```







