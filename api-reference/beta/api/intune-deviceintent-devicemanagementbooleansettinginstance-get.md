---
title: Obter deviceManagementBooleanSettingInstance
description: Leia as propriedades e as relações do objeto deviceManagementBooleanSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2bbd90c6fe52a908256185435e176558514f0bcf
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087801"
---
# <a name="get-devicemanagementbooleansettinginstance"></a><span data-ttu-id="6e2a2-103">Obter deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="6e2a2-103">Get deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="6e2a2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e2a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e2a2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e2a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e2a2-106">Leia as propriedades e as relações do objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="6e2a2-106">Read properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e2a2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e2a2-107">Prerequisites</span></span>
<span data-ttu-id="6e2a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e2a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e2a2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e2a2-110">Permission type</span></span>|<span data-ttu-id="6e2a2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e2a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e2a2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e2a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e2a2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e2a2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6e2a2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e2a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e2a2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e2a2-115">Not supported.</span></span>|
|<span data-ttu-id="6e2a2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e2a2-116">Application</span></span>|<span data-ttu-id="6e2a2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e2a2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e2a2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e2a2-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="6e2a2-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e2a2-119">Optional query parameters</span></span>
<span data-ttu-id="6e2a2-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e2a2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e2a2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e2a2-121">Request headers</span></span>
|<span data-ttu-id="6e2a2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e2a2-122">Header</span></span>|<span data-ttu-id="6e2a2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6e2a2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e2a2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e2a2-124">Authorization</span></span>|<span data-ttu-id="6e2a2-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e2a2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e2a2-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e2a2-126">Accept</span></span>|<span data-ttu-id="6e2a2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6e2a2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e2a2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e2a2-128">Request body</span></span>
<span data-ttu-id="6e2a2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e2a2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e2a2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e2a2-130">Response</span></span>
<span data-ttu-id="6e2a2-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e2a2-131">If successful, this method returns a `200 OK` response code and [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e2a2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e2a2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e2a2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e2a2-133">Request</span></span>
<span data-ttu-id="6e2a2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e2a2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="6e2a2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e2a2-135">Response</span></span>
<span data-ttu-id="6e2a2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e2a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






