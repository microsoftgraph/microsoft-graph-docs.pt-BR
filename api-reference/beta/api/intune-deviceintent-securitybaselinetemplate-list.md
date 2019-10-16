---
title: Listar securityBaselineTemplates
description: Listar Propriedades e relações dos objetos securityBaselineTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d13ea42549f3244720bfac6bb8ff1be93e6914f0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37531928"
---
# <a name="list-securitybaselinetemplates"></a><span data-ttu-id="dc3b0-103">Listar securityBaselineTemplates</span><span class="sxs-lookup"><span data-stu-id="dc3b0-103">List securityBaselineTemplates</span></span>

> <span data-ttu-id="dc3b0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc3b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc3b0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc3b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc3b0-106">Listar Propriedades e relações dos objetos [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="dc3b0-106">List properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc3b0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc3b0-107">Prerequisites</span></span>
<span data-ttu-id="dc3b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc3b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc3b0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc3b0-110">Permission type</span></span>|<span data-ttu-id="dc3b0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc3b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc3b0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc3b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc3b0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc3b0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dc3b0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc3b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc3b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc3b0-115">Not supported.</span></span>|
|<span data-ttu-id="dc3b0-116">Application</span><span class="sxs-lookup"><span data-stu-id="dc3b0-116">Application</span></span>|<span data-ttu-id="dc3b0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc3b0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc3b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc3b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="dc3b0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc3b0-119">Request headers</span></span>
|<span data-ttu-id="dc3b0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc3b0-120">Header</span></span>|<span data-ttu-id="dc3b0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dc3b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc3b0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc3b0-122">Authorization</span></span>|<span data-ttu-id="dc3b0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc3b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc3b0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc3b0-124">Accept</span></span>|<span data-ttu-id="dc3b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc3b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc3b0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc3b0-126">Request body</span></span>
<span data-ttu-id="dc3b0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc3b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc3b0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc3b0-128">Response</span></span>
<span data-ttu-id="dc3b0-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc3b0-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc3b0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc3b0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc3b0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc3b0-131">Request</span></span>
<span data-ttu-id="dc3b0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc3b0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates
```

### <a name="response"></a><span data-ttu-id="dc3b0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc3b0-133">Response</span></span>
<span data-ttu-id="dc3b0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc3b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 493

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineTemplate",
      "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
      "displayName": "Display Name value",
      "description": "Description value",
      "versionInfo": "Version Info value",
      "isDeprecated": true,
      "intentCount": 11,
      "templateType": "specializedDevices",
      "platformType": "androidForWork",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
    }
  ]
}
```






