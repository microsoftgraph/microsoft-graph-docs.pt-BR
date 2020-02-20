---
title: Listar deviceManagementIntentSettingCategories
description: Listar Propriedades e relações dos objetos deviceManagementIntentSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c96220e17c5752f7504b5d897f1c8444c550c46
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162404"
---
# <a name="list-devicemanagementintentsettingcategories"></a><span data-ttu-id="3d26b-103">Listar deviceManagementIntentSettingCategories</span><span class="sxs-lookup"><span data-stu-id="3d26b-103">List deviceManagementIntentSettingCategories</span></span>

> <span data-ttu-id="3d26b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d26b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d26b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d26b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d26b-106">Listar Propriedades e relações dos objetos [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="3d26b-106">List properties and relationships of the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d26b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d26b-107">Prerequisites</span></span>
<span data-ttu-id="3d26b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d26b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d26b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d26b-110">Permission type</span></span>|<span data-ttu-id="3d26b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3d26b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d26b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d26b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3d26b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d26b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3d26b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d26b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d26b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d26b-115">Not supported.</span></span>|
|<span data-ttu-id="3d26b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d26b-116">Application</span></span>|<span data-ttu-id="3d26b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d26b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d26b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d26b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="3d26b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d26b-119">Request headers</span></span>
|<span data-ttu-id="3d26b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d26b-120">Header</span></span>|<span data-ttu-id="3d26b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3d26b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d26b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d26b-122">Authorization</span></span>|<span data-ttu-id="3d26b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d26b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d26b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3d26b-124">Accept</span></span>|<span data-ttu-id="3d26b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3d26b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d26b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d26b-126">Request body</span></span>
<span data-ttu-id="3d26b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d26b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d26b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d26b-128">Response</span></span>
<span data-ttu-id="3d26b-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d26b-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d26b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d26b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d26b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d26b-131">Request</span></span>
<span data-ttu-id="3d26b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d26b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
```

### <a name="response"></a><span data-ttu-id="3d26b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d26b-133">Response</span></span>
<span data-ttu-id="3d26b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d26b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
      "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
      "displayName": "Display Name value",
      "hasRequiredSetting": true
    }
  ]
}
```





