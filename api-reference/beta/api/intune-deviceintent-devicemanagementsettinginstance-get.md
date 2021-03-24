---
title: Obter deviceManagementSettingInstance
description: Leia propriedades e relações do objeto deviceManagementSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3cdd115bdda349d6392aa49178682769ce756147
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128723"
---
# <a name="get-devicemanagementsettinginstance"></a><span data-ttu-id="f5764-103">Obter deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="f5764-103">Get deviceManagementSettingInstance</span></span>

<span data-ttu-id="f5764-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5764-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5764-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5764-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5764-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5764-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5764-107">Leia propriedades e relações do [objeto deviceManagementSettingInstance.](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="f5764-107">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5764-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5764-108">Prerequisites</span></span>
<span data-ttu-id="f5764-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5764-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5764-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5764-111">Permission type</span></span>|<span data-ttu-id="f5764-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5764-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5764-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5764-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5764-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5764-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5764-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5764-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5764-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5764-116">Not supported.</span></span>|
|<span data-ttu-id="f5764-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5764-117">Application</span></span>|<span data-ttu-id="f5764-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5764-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5764-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5764-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="f5764-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5764-120">Optional query parameters</span></span>
<span data-ttu-id="f5764-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5764-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5764-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5764-122">Request headers</span></span>
|<span data-ttu-id="f5764-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5764-123">Header</span></span>|<span data-ttu-id="f5764-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f5764-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5764-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5764-125">Authorization</span></span>|<span data-ttu-id="f5764-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5764-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5764-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5764-127">Accept</span></span>|<span data-ttu-id="f5764-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f5764-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5764-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5764-129">Request body</span></span>
<span data-ttu-id="f5764-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5764-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5764-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5764-131">Response</span></span>
<span data-ttu-id="f5764-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5764-132">If successful, this method returns a `200 OK` response code and [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5764-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5764-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5764-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5764-134">Request</span></span>
<span data-ttu-id="f5764-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5764-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="f5764-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5764-136">Response</span></span>
<span data-ttu-id="f5764-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5764-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
    "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value"
  }
}
```




