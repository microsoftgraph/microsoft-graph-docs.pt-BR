---
title: Listar deviceManagementSettingInstances
description: Listar Propriedades e relações dos objetos deviceManagementSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f922d5251c210da8a958e64bc40b99922718d717
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945547"
---
# <a name="list-devicemanagementsettinginstances"></a><span data-ttu-id="2df04-103">Listar deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="2df04-103">List deviceManagementSettingInstances</span></span>

> <span data-ttu-id="2df04-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2df04-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2df04-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2df04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2df04-106">Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="2df04-106">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2df04-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2df04-107">Prerequisites</span></span>
<span data-ttu-id="2df04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df04-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2df04-110">Permission type</span></span>|<span data-ttu-id="2df04-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2df04-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df04-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2df04-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2df04-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2df04-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2df04-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2df04-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df04-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df04-115">Not supported.</span></span>|
|<span data-ttu-id="2df04-116">Application</span><span class="sxs-lookup"><span data-stu-id="2df04-116">Application</span></span>|<span data-ttu-id="2df04-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2df04-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df04-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2df04-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2df04-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2df04-119">Request headers</span></span>
|<span data-ttu-id="2df04-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2df04-120">Header</span></span>|<span data-ttu-id="2df04-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2df04-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df04-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2df04-122">Authorization</span></span>|<span data-ttu-id="2df04-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2df04-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df04-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2df04-124">Accept</span></span>|<span data-ttu-id="2df04-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2df04-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df04-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2df04-126">Request body</span></span>
<span data-ttu-id="2df04-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2df04-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2df04-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df04-128">Response</span></span>
<span data-ttu-id="2df04-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2df04-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df04-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2df04-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2df04-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df04-131">Request</span></span>
<span data-ttu-id="2df04-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df04-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="2df04-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df04-133">Response</span></span>
<span data-ttu-id="2df04-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2df04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```





