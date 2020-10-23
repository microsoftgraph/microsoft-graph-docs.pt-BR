---
title: Listar deviceManagementIntegerSettingInstances
description: Listar Propriedades e relações dos objetos deviceManagementIntegerSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b055f20415d73483c08eabc0a4eb765ebf80edb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707385"
---
# <a name="list-devicemanagementintegersettinginstances"></a><span data-ttu-id="c2b2c-103">Listar deviceManagementIntegerSettingInstances</span><span class="sxs-lookup"><span data-stu-id="c2b2c-103">List deviceManagementIntegerSettingInstances</span></span>

<span data-ttu-id="c2b2c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2b2c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2b2c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2b2c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2b2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2b2c-107">Listar Propriedades e relações dos objetos [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="c2b2c-107">List properties and relationships of the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2b2c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c2b2c-108">Prerequisites</span></span>
<span data-ttu-id="c2b2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2b2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2b2c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2b2c-111">Permission type</span></span>|<span data-ttu-id="c2b2c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c2b2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2b2c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2b2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2b2c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c2b2c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2b2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2b2c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2b2c-116">Not supported.</span></span>|
|<span data-ttu-id="c2b2c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2b2c-117">Application</span></span>|<span data-ttu-id="c2b2c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2b2c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2b2c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c2b2c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2b2c-120">Request headers</span></span>
|<span data-ttu-id="c2b2c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2b2c-121">Header</span></span>|<span data-ttu-id="c2b2c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c2b2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2b2c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2b2c-123">Authorization</span></span>|<span data-ttu-id="c2b2c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2b2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2b2c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c2b2c-125">Accept</span></span>|<span data-ttu-id="c2b2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2b2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2b2c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2b2c-127">Request body</span></span>
<span data-ttu-id="c2b2c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2b2c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2b2c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2b2c-129">Response</span></span>
<span data-ttu-id="c2b2c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2b2c-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2b2c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2b2c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2b2c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2b2c-132">Request</span></span>
<span data-ttu-id="c2b2c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2b2c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="c2b2c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2b2c-134">Response</span></span>
<span data-ttu-id="c2b2c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2b2c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
      "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": 5
    }
  ]
}
```





