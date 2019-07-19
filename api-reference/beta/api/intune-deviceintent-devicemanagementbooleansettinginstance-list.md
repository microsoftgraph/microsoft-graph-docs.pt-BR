---
title: Listar deviceManagementBooleanSettingInstances
description: Listar Propriedades e relações dos objetos deviceManagementBooleanSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 099027f076b54ac1665e4b2e03813a16422300e0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960934"
---
# <a name="list-devicemanagementbooleansettinginstances"></a><span data-ttu-id="f5501-103">Listar deviceManagementBooleanSettingInstances</span><span class="sxs-lookup"><span data-stu-id="f5501-103">List deviceManagementBooleanSettingInstances</span></span>

> <span data-ttu-id="f5501-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5501-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5501-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5501-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5501-106">Listar Propriedades e relações dos objetos [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="f5501-106">List properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5501-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5501-107">Prerequisites</span></span>
<span data-ttu-id="f5501-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5501-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5501-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5501-110">Permission type</span></span>|<span data-ttu-id="f5501-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5501-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5501-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5501-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5501-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5501-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f5501-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5501-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5501-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5501-115">Not supported.</span></span>|
|<span data-ttu-id="f5501-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5501-116">Application</span></span>|<span data-ttu-id="f5501-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5501-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5501-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5501-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f5501-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5501-119">Request headers</span></span>
|<span data-ttu-id="f5501-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5501-120">Header</span></span>|<span data-ttu-id="f5501-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f5501-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5501-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5501-122">Authorization</span></span>|<span data-ttu-id="f5501-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5501-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5501-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5501-124">Accept</span></span>|<span data-ttu-id="f5501-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5501-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5501-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5501-126">Request body</span></span>
<span data-ttu-id="f5501-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5501-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5501-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5501-128">Response</span></span>
<span data-ttu-id="f5501-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5501-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5501-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5501-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5501-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5501-131">Request</span></span>
<span data-ttu-id="f5501-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5501-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="f5501-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5501-133">Response</span></span>
<span data-ttu-id="f5501-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5501-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





