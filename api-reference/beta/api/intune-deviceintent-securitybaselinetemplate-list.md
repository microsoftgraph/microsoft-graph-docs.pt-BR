---
title: Listar securityBaselineTemplates
description: Listar Propriedades e relações dos objetos securityBaselineTemplate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da244d8a31974c8620aa6c6888543dbd10b84c20
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177139"
---
# <a name="list-securitybaselinetemplates"></a><span data-ttu-id="b2836-103">Listar securityBaselineTemplates</span><span class="sxs-lookup"><span data-stu-id="b2836-103">List securityBaselineTemplates</span></span>

<span data-ttu-id="b2836-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2836-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2836-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2836-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2836-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2836-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2836-107">Listar Propriedades e relações dos objetos [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="b2836-107">List properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2836-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2836-108">Prerequisites</span></span>
<span data-ttu-id="b2836-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2836-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2836-111">Permission type</span></span>|<span data-ttu-id="b2836-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2836-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2836-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2836-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2836-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2836-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b2836-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2836-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2836-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2836-116">Not supported.</span></span>|
|<span data-ttu-id="b2836-117">Application</span><span class="sxs-lookup"><span data-stu-id="b2836-117">Application</span></span>|<span data-ttu-id="b2836-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2836-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2836-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2836-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="b2836-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2836-120">Request headers</span></span>
|<span data-ttu-id="b2836-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2836-121">Header</span></span>|<span data-ttu-id="b2836-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b2836-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2836-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2836-123">Authorization</span></span>|<span data-ttu-id="b2836-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2836-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2836-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2836-125">Accept</span></span>|<span data-ttu-id="b2836-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2836-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2836-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2836-127">Request body</span></span>
<span data-ttu-id="b2836-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2836-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2836-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2836-129">Response</span></span>
<span data-ttu-id="b2836-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2836-130">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2836-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2836-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2836-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2836-132">Request</span></span>
<span data-ttu-id="b2836-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2836-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates
```

### <a name="response"></a><span data-ttu-id="b2836-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2836-134">Response</span></span>
<span data-ttu-id="b2836-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2836-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

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
      "templateSubtype": "firewall",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
    }
  ]
}
```



