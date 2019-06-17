---
title: Listar deviceManagementCollectionSettingInstances
description: Listar Propriedades e relações dos objetos deviceManagementCollectionSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93b1edb40d77c89acd2354869add6bfffbb77257
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960766"
---
# <a name="list-devicemanagementcollectionsettinginstances"></a><span data-ttu-id="fb7b1-103">Listar deviceManagementCollectionSettingInstances</span><span class="sxs-lookup"><span data-stu-id="fb7b1-103">List deviceManagementCollectionSettingInstances</span></span>

> <span data-ttu-id="fb7b1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb7b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb7b1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb7b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb7b1-106">Listar Propriedades e relações dos objetos [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="fb7b1-106">List properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb7b1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb7b1-107">Prerequisites</span></span>
<span data-ttu-id="fb7b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb7b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb7b1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb7b1-110">Permission type</span></span>|<span data-ttu-id="fb7b1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb7b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb7b1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb7b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb7b1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb7b1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fb7b1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb7b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb7b1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb7b1-115">Not supported.</span></span>|
|<span data-ttu-id="fb7b1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb7b1-116">Application</span></span>|<span data-ttu-id="fb7b1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb7b1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb7b1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb7b1-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fb7b1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb7b1-119">Request headers</span></span>
|<span data-ttu-id="fb7b1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb7b1-120">Header</span></span>|<span data-ttu-id="fb7b1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fb7b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb7b1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb7b1-122">Authorization</span></span>|<span data-ttu-id="fb7b1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb7b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb7b1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb7b1-124">Accept</span></span>|<span data-ttu-id="fb7b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb7b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb7b1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb7b1-126">Request body</span></span>
<span data-ttu-id="fb7b1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb7b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb7b1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb7b1-128">Response</span></span>
<span data-ttu-id="fb7b1-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb7b1-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb7b1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb7b1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb7b1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb7b1-131">Request</span></span>
<span data-ttu-id="fb7b1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb7b1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="fb7b1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb7b1-133">Response</span></span>
<span data-ttu-id="fb7b1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb7b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
      "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```





