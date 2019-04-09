---
title: Obter deviceManagementIntentSettingCategory
description: Leia as propriedades e as relações do objeto deviceManagementIntentSettingCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79bfceede3dd2c3a433e0599b42283f9a62f0fc4
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522465"
---
# <a name="get-devicemanagementintentsettingcategory"></a><span data-ttu-id="8ac18-103">Obter deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="8ac18-103">Get deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="8ac18-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ac18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ac18-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ac18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ac18-106">Leia as propriedades e as relações do objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="8ac18-106">Read properties and relationships of the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ac18-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ac18-107">Prerequisites</span></span>
<span data-ttu-id="8ac18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ac18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ac18-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ac18-110">Permission type</span></span>|<span data-ttu-id="8ac18-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ac18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ac18-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ac18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ac18-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ac18-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8ac18-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ac18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ac18-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ac18-115">Not supported.</span></span>|
|<span data-ttu-id="8ac18-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ac18-116">Application</span></span>|<span data-ttu-id="8ac18-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ac18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ac18-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ac18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ac18-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ac18-119">Optional query parameters</span></span>
<span data-ttu-id="8ac18-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ac18-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ac18-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ac18-121">Request headers</span></span>
|<span data-ttu-id="8ac18-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ac18-122">Header</span></span>|<span data-ttu-id="8ac18-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8ac18-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ac18-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ac18-124">Authorization</span></span>|<span data-ttu-id="8ac18-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ac18-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ac18-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ac18-126">Accept</span></span>|<span data-ttu-id="8ac18-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8ac18-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ac18-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ac18-128">Request body</span></span>
<span data-ttu-id="8ac18-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ac18-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ac18-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ac18-130">Response</span></span>
<span data-ttu-id="8ac18-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ac18-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ac18-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ac18-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ac18-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ac18-133">Request</span></span>
<span data-ttu-id="8ac18-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ac18-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="8ac18-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ac18-135">Response</span></span>
<span data-ttu-id="8ac18-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ac18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 193

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
    "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
    "displayName": "Display Name value"
  }
}
```







