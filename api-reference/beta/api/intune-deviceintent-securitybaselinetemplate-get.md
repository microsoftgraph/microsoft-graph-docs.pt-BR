---
title: Obter securityBaselineTemplate
description: Leia as propriedades e as relações do objeto securityBaselineTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d407bd4c3884b60bf9b90b662f697c93bbc8af89
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814824"
---
# <a name="get-securitybaselinetemplate"></a><span data-ttu-id="3af51-103">Obter securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="3af51-103">Get securityBaselineTemplate</span></span>

> <span data-ttu-id="3af51-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3af51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3af51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3af51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3af51-106">Leia as propriedades e as relações do objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="3af51-106">Read properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3af51-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3af51-107">Prerequisites</span></span>
<span data-ttu-id="3af51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3af51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3af51-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3af51-110">Permission type</span></span>|<span data-ttu-id="3af51-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3af51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3af51-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3af51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3af51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3af51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3af51-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3af51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3af51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3af51-115">Not supported.</span></span>|
|<span data-ttu-id="3af51-116">Application</span><span class="sxs-lookup"><span data-stu-id="3af51-116">Application</span></span>|<span data-ttu-id="3af51-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3af51-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3af51-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3af51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3af51-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3af51-119">Optional query parameters</span></span>
<span data-ttu-id="3af51-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3af51-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3af51-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3af51-121">Request headers</span></span>
|<span data-ttu-id="3af51-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3af51-122">Header</span></span>|<span data-ttu-id="3af51-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3af51-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3af51-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3af51-124">Authorization</span></span>|<span data-ttu-id="3af51-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3af51-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3af51-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3af51-126">Accept</span></span>|<span data-ttu-id="3af51-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3af51-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3af51-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3af51-128">Request body</span></span>
<span data-ttu-id="3af51-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3af51-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3af51-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3af51-130">Response</span></span>
<span data-ttu-id="3af51-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3af51-131">If successful, this method returns a `200 OK` response code and [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3af51-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3af51-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3af51-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3af51-133">Request</span></span>
<span data-ttu-id="3af51-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3af51-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
```

### <a name="response"></a><span data-ttu-id="3af51-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3af51-135">Response</span></span>
<span data-ttu-id="3af51-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3af51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

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
    "platformType": "androidForWork",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
  }
}
```




