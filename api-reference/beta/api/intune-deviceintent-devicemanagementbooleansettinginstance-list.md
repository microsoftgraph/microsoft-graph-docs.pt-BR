---
title: Listar deviceManagementBooleanSettingInstances
description: Listar propriedades e relações dos objetos deviceManagementBooleanSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db46c2ce7704448c45eaaffb4ca46a9e6e4dd2a8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146591"
---
# <a name="list-devicemanagementbooleansettinginstances"></a><span data-ttu-id="83e4d-103">Listar deviceManagementBooleanSettingInstances</span><span class="sxs-lookup"><span data-stu-id="83e4d-103">List deviceManagementBooleanSettingInstances</span></span>

<span data-ttu-id="83e4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83e4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83e4d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83e4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83e4d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83e4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83e4d-107">Listar propriedades e relações dos [objetos deviceManagementBooleanSettingInstance.](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="83e4d-107">List properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83e4d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83e4d-108">Prerequisites</span></span>
<span data-ttu-id="83e4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83e4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83e4d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83e4d-111">Permission type</span></span>|<span data-ttu-id="83e4d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83e4d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83e4d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83e4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83e4d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e4d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83e4d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83e4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83e4d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83e4d-116">Not supported.</span></span>|
|<span data-ttu-id="83e4d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83e4d-117">Application</span></span>|<span data-ttu-id="83e4d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e4d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83e4d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83e4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="83e4d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83e4d-120">Request headers</span></span>
|<span data-ttu-id="83e4d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83e4d-121">Header</span></span>|<span data-ttu-id="83e4d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="83e4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83e4d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83e4d-123">Authorization</span></span>|<span data-ttu-id="83e4d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83e4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83e4d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83e4d-125">Accept</span></span>|<span data-ttu-id="83e4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83e4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83e4d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83e4d-127">Request body</span></span>
<span data-ttu-id="83e4d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83e4d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83e4d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="83e4d-129">Response</span></span>
<span data-ttu-id="83e4d-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83e4d-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83e4d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83e4d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="83e4d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83e4d-132">Request</span></span>
<span data-ttu-id="83e4d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83e4d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="83e4d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="83e4d-134">Response</span></span>
<span data-ttu-id="83e4d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83e4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
      "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": true
    }
  ]
}
```




