---
title: Obter securityBaselineTemplate
description: Leia as propriedades e as relações do objeto securityBaselineTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f853a38d4d95a047bd899a05d7b4333b15affbf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348960"
---
# <a name="get-securitybaselinetemplate"></a><span data-ttu-id="9f437-103">Obter securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="9f437-103">Get securityBaselineTemplate</span></span>

> <span data-ttu-id="9f437-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f437-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f437-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f437-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f437-106">Leia as propriedades e as relações do objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="9f437-106">Read properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f437-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f437-107">Prerequisites</span></span>
<span data-ttu-id="9f437-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f437-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f437-110">Permission type</span></span>|<span data-ttu-id="9f437-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f437-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f437-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f437-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f437-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f437-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9f437-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f437-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f437-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f437-115">Not supported.</span></span>|
|<span data-ttu-id="9f437-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f437-116">Application</span></span>|<span data-ttu-id="9f437-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f437-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f437-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f437-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f437-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9f437-119">Optional query parameters</span></span>
<span data-ttu-id="9f437-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9f437-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f437-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f437-121">Request headers</span></span>
|<span data-ttu-id="9f437-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f437-122">Header</span></span>|<span data-ttu-id="9f437-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9f437-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f437-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f437-124">Authorization</span></span>|<span data-ttu-id="9f437-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f437-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f437-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f437-126">Accept</span></span>|<span data-ttu-id="9f437-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9f437-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f437-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f437-128">Request body</span></span>
<span data-ttu-id="9f437-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f437-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f437-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f437-130">Response</span></span>
<span data-ttu-id="9f437-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f437-131">If successful, this method returns a `200 OK` response code and [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f437-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f437-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f437-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f437-133">Request</span></span>
<span data-ttu-id="9f437-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f437-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
```

### <a name="response"></a><span data-ttu-id="9f437-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f437-135">Response</span></span>
<span data-ttu-id="9f437-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f437-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 420

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineTemplate",
    "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
    "displayName": "Display Name value",
    "description": "Description value",
    "versionInfo": "Version Info value",
    "isDeprecated": true,
    "intentCount": 11,
    "templateType": "specializedDevices",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
  }
}
```






